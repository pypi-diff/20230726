# Comparing `tmp/torch_uncertainty-0.1.2.tar.gz` & `tmp/torch_uncertainty-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_uncertainty-0.1.2.tar", max compression
+gzip compressed data, was "torch_uncertainty-0.1.3.tar", max compression
```

## Comparing `torch_uncertainty-0.1.2.tar` & `torch_uncertainty-0.1.3.tar`

### file list

```diff
@@ -1,66 +1,88 @@
--rw-r--r--   0        0        0    11363 2023-06-05 07:26:13.703778 torch_uncertainty-0.1.2/LICENSE
--rw-r--r--   0        0        0     3519 2023-06-05 07:26:13.703778 torch_uncertainty-0.1.2/README.md
--rw-r--r--   0        0        0     2057 2023-06-05 07:26:13.707778 torch_uncertainty-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3159 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/__init__.py
--rw-r--r--   0        0        0      107 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/__init__.py
--rw-r--r--   0        0        0     7903 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/resnet.py
--rw-r--r--   0        0        0     6918 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/wideresnet.py
--rw-r--r--   0        0        0     1273 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/baselines/utils/parser_addons.py
--rw-r--r--   0        0        0      221 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/__init__.py
--rw-r--r--   0        0        0     6825 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/cifar10.py
--rw-r--r--   0        0        0     7037 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/cifar100.py
--rw-r--r--   0        0        0     7576 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/imagenet.py
--rw-r--r--   0        0        0     4705 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/mnist.py
--rw-r--r--   0        0        0     4752 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datamodules/tiny_imagenet.py
--rw-r--r--   0        0        0      216 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/__init__.py
--rw-r--r--   0        0        0      771 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/aggregated_dataset.py
--rw-r--r--   0        0        0       89 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/__init__.py
--rw-r--r--   0        0        0     7570 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/cifar_c.py
--rw-r--r--   0        0        0     2700 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/cifar_h.py
--rw-r--r--   0        0        0     1969 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/fractals.py
--rw-r--r--   0        0        0      157 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/__init__.py
--rw-r--r--   0        0        0     2446 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/base.py
--rw-r--r--   0        0        0      313 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/imagenet_a.py
--rw-r--r--   0        0        0      313 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/imagenet_o.py
--rw-r--r--   0        0        0      313 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/imagenet_r.py
--rw-r--r--   0        0        0     5007 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet/tiny_imagenet.py
--rw-r--r--   0        0        0     1606 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/datasets/imagenet_r.py
--rw-r--r--   0        0        0      182 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/layers/__init__.py
--rw-r--r--   0        0        0    15104 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/layers/batchens_layers.py
--rw-r--r--   0        0        0     9929 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/layers/masksembles_layers.py
--rw-r--r--   0        0        0     9048 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/layers/packed_layers.py
--rw-r--r--   0        0        0      340 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/__init__.py
--rw-r--r--   0        0        0     4042 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/brier_score.py
--rw-r--r--   0        0        0     3456 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/disagreement.py
--rw-r--r--   0        0        0     3098 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/entropy.py
--rw-r--r--   0        0        0     4060 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/fpr95.py
--rw-r--r--   0        0        0     3829 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/jensen_shannon_divergence.py
--rw-r--r--   0        0        0     3376 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/mutual_information.py
--rw-r--r--   0        0        0     3149 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/nll.py
--rw-r--r--   0        0        0     2656 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/metrics/variation_ratio.py
--rw-r--r--   0        0        0        0 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/__init__.py
--rw-r--r--   0        0        0      101 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/__init__.py
--rw-r--r--   0        0        0    12044 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/batched.py
--rw-r--r--   0        0        0    12641 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/masked.py
--rw-r--r--   0        0        0    16040 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/packed.py
--rw-r--r--   0        0        0    10540 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/std.py
--rw-r--r--   0        0        0      101 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/__init__.py
--rw-r--r--   0        0        0     6145 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/batched.py
--rw-r--r--   0        0        0     6441 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/masked.py
--rw-r--r--   0        0        0     7362 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/packed.py
--rw-r--r--   0        0        0     5420 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/std.py
--rw-r--r--   0        0        0     7527 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/optimization_procedures.py
--rw-r--r--   0        0        0       65 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/post_processing/__init__.py
--rw-r--r--   0        0        0     3426 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/post_processing/temperature_scaler.py
--rw-r--r--   0        0        0        0 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/routines/__init__.py
--rw-r--r--   0        0        0    14608 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/routines/classification.py
--rw-r--r--   0        0        0      405 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/transforms/__init__.py
--rw-r--r--   0        0        0     1255 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/transforms/cutout.py
--rw-r--r--   0        0        0     4351 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/transforms/pixmix.py
--rw-r--r--   0        0        0     6939 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/transforms/transforms.py
--rw-r--r--   0        0        0       77 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/utils/__init__.py
--rw-r--r--   0        0        0     1313 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/utils/checkpoints.py
--rw-r--r--   0        0        0      210 2023-06-05 07:26:13.711778 torch_uncertainty-0.1.2/torch_uncertainty/utils/hub.py
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.2/setup.py
--rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11363 2023-07-26 07:52:59.177707 torch_uncertainty-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3707 2023-07-26 07:52:59.177707 torch_uncertainty-0.1.3/README.md
+-rw-r--r--   0        0        0     2171 2023-07-26 07:52:59.181707 torch_uncertainty-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4090 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/__init__.py
+-rw-r--r--   0        0        0       98 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/classification/__init__.py
+-rw-r--r--   0        0        0     8900 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/classification/resnet.py
+-rw-r--r--   0        0        0     6874 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/classification/vgg.py
+-rw-r--r--   0        0        0     7895 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/classification/wideresnet.py
+-rw-r--r--   0        0        0     3426 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/deep_ensembles.py
+-rw-r--r--   0        0        0       36 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/regression/__init__.py
+-rw-r--r--   0        0        0     3633 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/regression/mlp.py
+-rw-r--r--   0        0        0     2584 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/baselines/utils/parser_addons.py
+-rw-r--r--   0        0        0      263 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datamodules/__init__.py
+-rw-r--r--   0        0        0     8570 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datamodules/cifar10.py
+-rw-r--r--   0        0        0     9013 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datamodules/cifar100.py
+-rw-r--r--   0        0        0     8705 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datamodules/imagenet.py
+-rw-r--r--   0        0        0     6153 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datamodules/mnist.py
+-rw-r--r--   0        0        0     5460 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datamodules/tiny_imagenet.py
+-rw-r--r--   0        0        0     4658 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datamodules/uci_regression.py
+-rw-r--r--   0        0        0      258 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/__init__.py
+-rw-r--r--   0        0        0      766 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/aggregated_dataset.py
+-rw-r--r--   0        0        0       89 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/cifar/__init__.py
+-rw-r--r--   0        0        0     8736 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/cifar/cifar_c.py
+-rw-r--r--   0        0        0     2812 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/cifar/cifar_h.py
+-rw-r--r--   0        0        0     4375 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/cifar/cifar_n.py
+-rw-r--r--   0        0        0     1971 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/fractals.py
+-rw-r--r--   0        0        0      157 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/imagenet/__init__.py
+-rw-r--r--   0        0        0     4731 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/imagenet/base.py
+-rw-r--r--   0        0        0      313 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/imagenet/imagenet_a.py
+-rw-r--r--   0        0        0     1150 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/imagenet/imagenet_c.py
+-rw-r--r--   0        0        0      313 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/imagenet/imagenet_o.py
+-rw-r--r--   0        0        0      313 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/imagenet/imagenet_r.py
+-rw-r--r--   0        0        0     3898 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/imagenet/tiny_imagenet.py
+-rw-r--r--   0        0        0    10426 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/datasets/uci_regression.py
+-rw-r--r--   0        0        0      262 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/layers/__init__.py
+-rw-r--r--   0        0        0    15104 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/layers/batchens_layers.py
+-rw-r--r--   0        0        0      188 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/layers/bayesian_layers/__init__.py
+-rw-r--r--   0        0        0    15038 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/layers/bayesian_layers/bayes_conv.py
+-rw-r--r--   0        0        0     5378 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/layers/bayesian_layers/bayes_linear.py
+-rw-r--r--   0        0        0     2084 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/layers/bayesian_layers/sampler.py
+-rw-r--r--   0        0        0     9929 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/layers/masksembles_layers.py
+-rw-r--r--   0        0        0    11169 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/layers/packed_layers.py
+-rw-r--r--   0        0        0     2326 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/losses.py
+-rw-r--r--   0        0        0      371 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/__init__.py
+-rw-r--r--   0        0        0     4273 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/brier_score.py
+-rw-r--r--   0        0        0     3456 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/disagreement.py
+-rw-r--r--   0        0        0     3098 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/entropy.py
+-rw-r--r--   0        0        0     4094 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/fpr95.py
+-rw-r--r--   0        0        0     3829 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/jensen_shannon_divergence.py
+-rw-r--r--   0        0        0     3376 2023-07-26 07:52:59.185707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/mutual_information.py
+-rw-r--r--   0        0        0     4880 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/nll.py
+-rw-r--r--   0        0        0     2695 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/metrics/variation_ratio.py
+-rw-r--r--   0        0        0       58 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/__init__.py
+-rw-r--r--   0        0        0     1852 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/deep_ensembles.py
+-rw-r--r--   0        0        0     5343 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/lenet.py
+-rw-r--r--   0        0        0     5204 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/mlp.py
+-rw-r--r--   0        0        0      101 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/__init__.py
+-rw-r--r--   0        0        0    11855 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/batched.py
+-rw-r--r--   0        0        0    12465 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/masked.py
+-rw-r--r--   0        0        0    17301 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/packed.py
+-rw-r--r--   0        0        0    10337 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/std.py
+-rw-r--r--   0        0        0      709 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/utils.py
+-rw-r--r--   0        0        0       56 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/vgg/__init__.py
+-rw-r--r--   0        0        0     4517 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/vgg/base.py
+-rw-r--r--   0        0        0      481 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/vgg/configs.py
+-rw-r--r--   0        0        0     2659 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/vgg/packed.py
+-rw-r--r--   0        0        0     1689 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/vgg/std.py
+-rw-r--r--   0        0        0      101 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/__init__.py
+-rw-r--r--   0        0        0     6092 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/batched.py
+-rw-r--r--   0        0        0     6388 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/masked.py
+-rw-r--r--   0        0        0     7309 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/packed.py
+-rw-r--r--   0        0        0     5367 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/std.py
+-rw-r--r--   0        0        0     9277 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/optimization_procedures.py
+-rw-r--r--   0        0        0       65 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/post_processing/__init__.py
+-rw-r--r--   0        0        0     4712 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/post_processing/temperature_scaler.py
+-rw-r--r--   0        0        0        0 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/routines/__init__.py
+-rw-r--r--   0        0        0    17175 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/routines/classification.py
+-rw-r--r--   0        0        0     8314 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/routines/regression.py
+-rw-r--r--   0        0        0      405 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/transforms/__init__.py
+-rw-r--r--   0        0        0     1255 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/transforms/cutout.py
+-rw-r--r--   0        0        0     4463 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/transforms/pixmix.py
+-rw-r--r--   0        0        0     6879 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/transforms/transforms.py
+-rw-r--r--   0        0        0       77 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/utils/__init__.py
+-rw-r--r--   0        0        0     1313 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/utils/checkpoints.py
+-rw-r--r--   0        0        0      867 2023-07-26 07:52:59.189707 torch_uncertainty-0.1.3/torch_uncertainty/utils/hub.py
+-rw-r--r--   0        0        0     5365 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.3/setup.py
+-rw-r--r--   0        0        0     4761 1970-01-01 00:00:00.000000 torch_uncertainty-0.1.3/PKG-INFO
```

### Comparing `torch_uncertainty-0.1.2/LICENSE` & `torch_uncertainty-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/README.md` & `torch_uncertainty-0.1.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,37 +5,39 @@
 [![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty)
 [![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml)
 [![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/)
 [![Code Coverage](https://codecov.io/github/ENSTA-U2IS/torch-uncertainty/coverage.svg?branch=master)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 </div>
 
-_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.
+_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It aims at including as many methods as possible, so reach out to add yours!
 
 :construction: _TorchUncertainty_ is in early development :construction: - expect massive changes but do reach out to us and contribute if you are interested by the project!
 
 ---
 
 This package provides a multi-level API, including:
 
 - ready-to-train baselines on research datasets, such as ImageNet and CIFAR
 - baselines available for training on your datasets
 - [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR (work in progress 🚧).
 - layers available for use in your networks
-- post-processing methods such as temperature scaling
+- scikit-learn style post-processing methods such as Temperature Scaling
+
+See the [Reference page](https://torch-uncertainty.github.io/references.html) or the [API reference](https://torch-uncertainty.github.io/api.html) for a more exhaustive list of the implemented methods, datasets, metrics, etc.
 
 ## Installation
 
-The package can be installed from PyPI:
+Install the desired pytorch version in your environment. Then, the package can be installed from PyPI:
 
 ```sh
 pip install torch-uncertainty
 ```
 
-To contribute, install the package from source following the instructions of the [dedicated page](https://torch-uncertainty.github.io/installation.html) in the documentation and activate the pre-commit hooks with `pre-commit install`.
+If you aim to contribute (thank you!), have a look at the [contribution page](https://torch-uncertainty.github.io/contributing.html).
 
 ## Getting Started and Documentation
 
 Please find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).
 
 A quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).
 
@@ -45,26 +47,27 @@
 
 To date, the following baselines are implemented:
 
 - Deep Ensembles
 - BatchEnsemble
 - Masksembles
 - Packed-Ensembles (see [blog post](https://medium.com/@adrien.lafage/make-your-neural-networks-more-reliable-with-packed-ensembles-7ad0b737a873))
+- Bayesian Neural Networks
 
 ### Post-processing methods
 
 To date, the following post-processing methods are implemented:
 
 - Temperature scaling
 
 ## Tutorials
 
 ## Awesome Uncertainty repositories
 
-You may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).
+You may find a lot of papers about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).
 
 ## Other References
 
 This package also contains the official implementation of Packed-Ensembles.
 
 If you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):
```

### Comparing `torch_uncertainty-0.1.2/pyproject.toml` & `torch_uncertainty-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 [tool.poetry]
 name = "torch_uncertainty"
-version = "0.1.2"
+version = "0.1.3"
 description = "A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques."
 authors = [
     "ENSTA U2IS <olivier.laurent@ensta-paris.fr>",
     "Adrien Lafage <adrienlafage@outlook.com>",
     "Olivier Laurent <olivier.ar.laurent@gmail.com>",
 ]
 license = "Apache-2.0"
 keywords = ["deep-learning", "pytorch", "uncertainty", "ensembles", "uncertainty-quantification", "predictive-uncertainty", "reliable-ai", "deep-learning-uncertainty"]
 readme = "README.md"
 packages = [{include = "torch_uncertainty"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
+timm = ">=0.6.12"
 pytorch-lightning = "^1.9.0"
-tensorboard = "^2.11.2"
-einops = "^0.6.0"
-torchinfo = "^1.7.1"
-torchvision = "^0.14.1"
-timm = "^0.6.12"
+tensorboard = ">=2.11.2"
+einops = ">=0.6.0"
+torchinfo = ">=1.7.1"
 scipy = "^1.10.0"
 huggingface-hub = "^0.14.1"
+pandas = "^2.0.3"
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
-mypy = "^0.991"
 pytest-cov = "^4.0.0"
 pre-commit = "^3.0.4"
 pre-commit-hooks = "^4.4.0"
 cli-test-helpers = "^3.2.0"
 
+[tool.poetry.group.docs]
+optional = true
+
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.1.3"
 pytorch-sphinx-theme = {git = "https://github.com/torch-uncertainty/pytorch_sphinx_theme"}
 sphinx-copybutton = "^0.5.1"
-sphinx-gallery = "^0.12.2"
+sphinx-gallery = {git = "https://github.com/sphinx-gallery/sphinx-gallery"}
 matplotlib = "^3.7.1"
 sphinx-design = "^0.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/__init__.py` & `torch_uncertainty-0.1.3/torch_uncertainty/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # fmt: off
 # flake8: noqa
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
-from typing import Type, Union
+from typing import Dict, Optional, Type, Union
 
 import pytorch_lightning as pl
 import torch
 from pytorch_lightning.callbacks import LearningRateMonitor
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 from pytorch_lightning.callbacks.model_checkpoint import ModelCheckpoint
 from pytorch_lightning.loggers.tensorboard import TensorBoardLogger
@@ -15,54 +15,82 @@
 import numpy as np
 
 from .utils import get_version
 
 
 # fmt: on
 def init_args(
-    network: Type[pl.LightningModule], datamodule: Type[pl.LightningDataModule]
+    network: Optional[Type[pl.LightningModule]] = None,
+    datamodule: Optional[Type[pl.LightningDataModule]] = None,
 ) -> Namespace:
     parser = ArgumentParser("torch-uncertainty")
-    parser.add_argument("--seed", type=int, default=None)
-    parser.add_argument("--test", type=int, default=None)
-    parser.add_argument("--summary", dest="summary", action="store_true")
+    parser.add_argument(
+        "--seed",
+        type=int,
+        default=None,
+        help="Random seed to make the training deterministic.",
+    )
+    parser.add_argument(
+        "--test",
+        type=int,
+        default=None,
+        help="Run in test mode. Set to the checkpoint version number to test.",
+    )
+    parser.add_argument(
+        "--summary",
+        dest="summary",
+        action="store_true",
+        help="Print model summary",
+    )
     parser.add_argument("--log_graph", dest="log_graph", action="store_true")
     parser.add_argument(
         "--channels_last",
         action="store_true",
         help="Use channels last memory format",
     )
 
     parser = pl.Trainer.add_argparse_args(parser)
-    parser = datamodule.add_argparse_args(parser)
-    parser = network.add_model_specific_args(parser)
-    args = parser.parse_args()
+    if network is not None:
+        parser = network.add_model_specific_args(parser)
+
+    if datamodule is not None:
+        parser = datamodule.add_argparse_args(parser)
 
-    return args
+    return parser.parse_args()
 
 
-def cls_main(
+def cli_main(
     network: pl.LightningModule,
     datamodule: pl.LightningDataModule,
     root: Union[Path, str],
     net_name: str,
     args: Namespace,
-) -> None:
+) -> Dict:
     if isinstance(root, str):
         root = Path(root)
 
-    if args.max_epochs is None:
+    training_task = datamodule.training_task
+    if training_task == "classification":
+        monitor = "hp/val_acc"
+        mode = "max"
+    elif training_task == "regression":
+        monitor = "hp/val_mse"
+        mode = "min"
+    else:
+        raise ValueError("Unknown problem type.")
+
+    if args.test is None and args.max_epochs is None:
         print(
             "Setting max_epochs to 1 for testing purposes. Set max_epochs "
             "manually to train the model."
         )
         args.max_epochs = 1
 
     if isinstance(args.seed, int):
-        pl.seed_everything(args.seed)
+        pl.seed_everything(args.seed, workers=True)
 
     if args.channels_last:
         network = network.to(memory_format=torch.channels_last)
 
     # logger
     tb_logger = TensorBoardLogger(
         str(root / "logs"),
@@ -70,38 +98,45 @@
         default_hp_metric=False,
         log_graph=args.log_graph,
         version=args.test,
     )
 
     # callbacks
     save_checkpoints = ModelCheckpoint(
-        monitor="hp/val_acc",
-        mode="max",
+        monitor=monitor,
+        mode=mode,
         save_last=True,
         save_weights_only=True,
     )
 
     # Select the best model, monitor the lr and stop if NaN
     callbacks = [
         save_checkpoints,
         LearningRateMonitor(logging_interval="step"),
-        EarlyStopping(monitor="hp/val_nll", patience=np.inf, check_finite=True),
+        EarlyStopping(monitor=monitor, patience=np.inf, check_finite=True),
     ]
     # trainer
     trainer = pl.Trainer.from_argparse_args(
         args,
         callbacks=callbacks,
         logger=tb_logger,
         deterministic=(args.seed is not None),
     )
 
     if args.summary:
         summary(network, input_size=list(datamodule.input_shape).insert(0, 1))
+        test_values = {}
     elif args.test is not None:
-        ckpt_file, _ = get_version(
-            root=(root / "logs" / net_name), version=args.test
-        )
-        trainer.test(network, datamodule=datamodule, ckpt_path=str(ckpt_file))
+        if args.test >= 0:
+            ckpt_file, _ = get_version(
+                root=(root / "logs" / net_name), version=args.test
+            )
+            test_values = trainer.test(
+                network, datamodule=datamodule, ckpt_path=str(ckpt_file)
+            )
+        else:
+            test_values = trainer.test(network, datamodule=datamodule)
     else:
         # training and testing
         trainer.fit(network, datamodule)
-        trainer.test(datamodule=datamodule, ckpt_path="best")
+        test_values = trainer.test(datamodule=datamodule, ckpt_path="best")
+    return test_values
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/resnet.py` & `torch_uncertainty-0.1.3/torch_uncertainty/baselines/classification/resnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # fmt: off
 from argparse import ArgumentParser, BooleanOptionalAction
-from typing import Any, Literal, Optional
+from pathlib import Path
+from typing import Any, Literal, Optional, Type, Union
 
+import torch
 import torch.nn as nn
 from pytorch_lightning import LightningModule
+from pytorch_lightning.core.saving import (
+    load_hparams_from_tags_csv,
+    load_hparams_from_yaml,
+)
 
 from ...models.resnet import (
     batched_resnet18,
     batched_resnet34,
     batched_resnet50,
     batched_resnet101,
     batched_resnet152,
@@ -64,16 +70,16 @@
 
             - ``18``: ResNet-18
             - ``32``: ResNet-32
             - ``50``: ResNet-50
             - ``101``: ResNet-101
             - ``152``: ResNet-152
 
-        imagenet_structure (bool, optional): Whether to use the ImageNet
-            structure. Defaults to ``True``.
+        style (str, optional): Which ResNet style to use. Defaults to
+        ``imagenet``.
         num_estimators (int, optional): Number of estimators in the ensemble.
             Only used if :attr:`version` is either ``"packed"``, ``"batched"``
             or ``"masked"`` Defaults to ``None``.
         groups (int, optional): Number of groups in convolutions. Defaults to
             ``1``.
         scale (float, optional): Expansion factor affecting the width of the
             estimators. Only used if :attr:`version` is ``"masked"``. Defaults
@@ -132,35 +138,35 @@
     }
     archs = [18, 34, 50, 101, 152]
 
     def __new__(
         cls,
         num_classes: int,
         in_channels: int,
-        loss: nn.Module,
+        loss: Type[nn.Module],
         optimization_procedure: Any,
         version: Literal["vanilla", "packed", "batched", "masked"],
         arch: int,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
         num_estimators: Optional[int] = None,
-        groups: Optional[int] = 1,
+        groups: int = 1,
         scale: Optional[float] = None,
         alpha: Optional[float] = None,
-        gamma: Optional[int] = 1,
+        gamma: int = 1,
         use_entropy: bool = False,
         use_logits: bool = False,
         use_mi: bool = False,
         use_variation_ratio: bool = False,
         pretrained: bool = False,
         **kwargs,
     ) -> LightningModule:
         params = {
             "in_channels": in_channels,
             "num_classes": num_classes,
-            "imagenet_structure": imagenet_structure,
+            "style": style,
             "groups": groups,
         }
 
         if version not in cls.versions.keys():
             raise ValueError(f"Unknown version: {version}")
 
         if version == "packed":
@@ -184,14 +190,15 @@
                     "num_estimators": num_estimators,
                     "scale": scale,
                 }
             )
 
         model = cls.versions[version][cls.archs.index(arch)](**params)
         kwargs.update(params)
+        kwargs.update({"version": version, "arch": arch})
         # routine specific parameters
         if version in cls.single:
             return ClassificationSingle(
                 model=model,
                 loss=loss,
                 optimization_procedure=optimization_procedure,
                 use_entropy=use_entropy,
@@ -207,14 +214,38 @@
                 use_logits=use_logits,
                 use_mi=use_mi,
                 use_variation_ratio=use_variation_ratio,
                 **kwargs,
             )
 
     @classmethod
+    def load_from_checkpoint(
+        cls,
+        checkpoint_path: Union[str, Path],
+        hparams_file: Union[str, Path],
+        **kwargs,
+    ) -> LightningModule:  # coverage: ignore
+        if hparams_file is not None:
+            extension = str(hparams_file).split(".")[-1]
+            if extension.lower() == "csv":
+                hparams = load_hparams_from_tags_csv(hparams_file)
+            elif extension.lower() in ("yml", "yaml"):
+                hparams = load_hparams_from_yaml(hparams_file)
+            else:
+                raise ValueError(
+                    ".csv, .yml or .yaml is required for `hparams_file`"
+                )
+
+        hparams.update(kwargs)
+        checkpoint = torch.load(checkpoint_path)
+        obj = cls(**hparams)
+        obj.load_state_dict(checkpoint["state_dict"])
+        return obj
+
+    @classmethod
     def add_model_specific_args(cls, parser: ArgumentParser) -> ArgumentParser:
         parser = ClassificationEnsemble.add_model_specific_args(parser)
         parser = add_resnet_specific_args(parser)
         parser = add_packed_specific_args(parser)
         parser = add_masked_specific_args(parser)
         parser.add_argument(
             "--version",
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/baselines/classification/wideresnet.py` & `torch_uncertainty-0.1.3/torch_uncertainty/baselines/classification/wideresnet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # fmt: off
 from argparse import ArgumentParser, BooleanOptionalAction
-from typing import Any, Literal, Optional
+from pathlib import Path
+from typing import Any, Literal, Optional, Type, Union
 
+import torch
 import torch.nn as nn
 from pytorch_lightning import LightningModule
+from pytorch_lightning.core.saving import (
+    load_hparams_from_tags_csv,
+    load_hparams_from_yaml,
+)
 
 from ...models.wideresnet import (
     batched_wideresnet28x10,
     masked_wideresnet28x10,
     packed_wideresnet28x10,
     wideresnet28x10,
 )
@@ -39,16 +45,16 @@
             Determines which Wide-ResNet version to use:
 
             - ``"vanilla"``: original Wide-ResNet
             - ``"packed"``: Packed-Ensembles Wide-ResNet
             - ``"batched"``: BatchEnsemble Wide-ResNet
             - ``"masked"``: Masksemble Wide-ResNet
 
-        imagenet_structure (bool, optional): Whether to use the ImageNet
-            structure. Defaults to ``True``.
+        style (bool, optional): (str, optional): Which ResNet style to use.
+        Defaults to ``imagenet``.
         num_estimators (int, optional): Number of estimators in the ensemble.
             Only used if :attr:`version` is either ``"packed"``, ``"batched"``
             or ``"masked"`` Defaults to ``None``.
         groups (int, optional): Number of groups in convolutions. Defaults to
             ``1``.
         scale (float, optional): Expansion factor affecting the width of the
             estimators. Only used if :attr:`version` is ``"masked"``. Defaults
@@ -88,18 +94,18 @@
         "masked": [masked_wideresnet28x10],
     }
 
     def __new__(
         cls,
         num_classes: int,
         in_channels: int,
-        loss: nn.Module,
+        loss: Type[nn.Module],
         optimization_procedure: Any,
         version: Literal["vanilla", "packed", "batched", "masked"],
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
         num_estimators: Optional[int] = None,
         groups: Optional[int] = None,
         scale: Optional[float] = None,
         alpha: Optional[int] = None,
         gamma: Optional[int] = None,
         use_entropy: bool = False,
         use_logits: bool = False,
@@ -107,15 +113,15 @@
         use_variation_ratio: bool = False,
         # pretrained: bool = False,
         **kwargs,
     ) -> LightningModule:
         params = {
             "in_channels": in_channels,
             "num_classes": num_classes,
-            "imagenet_structure": imagenet_structure,
+            "style": style,
             "groups": groups,
         }
 
         if version not in cls.versions.keys():
             raise ValueError(f"Unknown version: {version}")
 
         # version specific params
@@ -162,14 +168,38 @@
                 use_logits=use_logits,
                 use_mi=use_mi,
                 use_variation_ratio=use_variation_ratio,
                 **kwargs,
             )
 
     @classmethod
+    def load_from_checkpoint(
+        cls,
+        checkpoint_path: Union[str, Path],
+        hparams_file: Union[str, Path],
+        **kwargs,
+    ) -> LightningModule:  # coverage: ignore
+        if hparams_file is not None:
+            extension = str(hparams_file).split(".")[-1]
+            if extension.lower() == "csv":
+                hparams = load_hparams_from_tags_csv(hparams_file)
+            elif extension.lower() in ("yml", "yaml"):
+                hparams = load_hparams_from_yaml(hparams_file)
+            else:
+                raise ValueError(
+                    ".csv, .yml or .yaml is required for `hparams_file`"
+                )
+
+        hparams.update(kwargs)
+        checkpoint = torch.load(checkpoint_path)
+        obj = cls(**hparams)
+        obj.load_state_dict(checkpoint["state_dict"])
+        return obj
+
+    @classmethod
     def add_model_specific_args(cls, parser: ArgumentParser) -> ArgumentParser:
         parser = ClassificationEnsemble.add_model_specific_args(parser)
         parser = add_wideresnet_specific_args(parser)
         parser = add_packed_specific_args(parser)
         parser = add_masked_specific_args(parser)
         parser.add_argument(
             "--version",
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/baselines/utils/parser_addons.py` & `torch_uncertainty-0.1.3/torch_uncertainty/baselines/utils/parser_addons.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,95 @@
 # fmt: off
 from argparse import ArgumentParser
 
 
 # fmt: on
 def add_resnet_specific_args(parser: ArgumentParser) -> ArgumentParser:
+    # style_choices = ["cifar", "imagenet", "robust"]
+    archs = [18, 34, 50, 101, 152]
     parser.add_argument(
         "--arch",
         type=int,
-        choices=[18, 34, 50, 101, 152],
+        choices=archs,
         default=18,
-        help=f"Architecture of ResNet. Choose among: {[18, 34, 50, 101, 152]}",
+        help=f"Architecture of ResNet. Choose among: {archs}",
     )
+    # parser.add_argument(
+    #     "--style",
+    #     type=str,
+    #     choices=style_choices,
+    #     default="imagenet",
+    #     help=f"Variation of ResNet. Choose among: {style_choices}",
+    # )
     parser.add_argument(
         "--groups",
         type=int,
         default=1,
         help="Number of groups",
     )
     return parser
 
 
+def add_vgg_specific_args(parser: ArgumentParser) -> ArgumentParser:
+    # style_choices = ["cifar", "imagenet", "robust"]
+    archs = [11, 13, 16, 19]
+    parser.add_argument(
+        "--arch",
+        type=int,
+        choices=archs,
+        default=11,
+        help=f"Architecture of VGG. Choose among: {archs}",
+    )
+    parser.add_argument(
+        "--groups",
+        type=int,
+        default=1,
+        help="Number of groups",
+    )
+    parser.add_argument(
+        "--dropout",
+        type=float,
+        default=0.1,
+        help="Dropout rate",
+    )
+    return parser
+
+
 def add_wideresnet_specific_args(parser: ArgumentParser) -> ArgumentParser:
+    # style_choices = ["cifar", "imagenet"]
+    # parser.add_argument(
+    #     "--style",
+    #     type=str,
+    #     choices=style_choices,
+    #     default="imagenet",
+    #     help=f"Variation of ResNet. Choose among: {style_choices}",
+    # )
     parser.add_argument(
         "--groups",
         type=int,
         default=1,
         help="Number of groups",
     )
     return parser
 
 
+def add_mlp_specific_args(parser: ArgumentParser) -> ArgumentParser:
+    parser.add_argument(
+        "--dropout",
+        type=float,
+        default=0.1,
+        help="Dropout rate",
+    )
+    return parser
+
+
 def add_packed_specific_args(parser: ArgumentParser) -> ArgumentParser:
     parser.add_argument(
         "--alpha",
-        type=float,
+        type=int,
         default=None,
         help="Alpha for Packed-Ensembles",
     )
     parser.add_argument(
         "--gamma",
         type=int,
         default=1,
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/cifar10.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datamodules/cifar10.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,74 @@
 # fmt: off
 from argparse import ArgumentParser
 from pathlib import Path
-from typing import Any, List, Optional, Union
+from typing import Any, List, Literal, Optional, Union
 
 import torch.nn as nn
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
 from timm.data.auto_augment import rand_augment_transform
 from torch.utils.data import DataLoader, Dataset, random_split
 from torchvision.datasets import CIFAR10, SVHN
 
 from ..datasets import CIFAR10_C, CIFAR10_H, AggregatedDataset
 from ..transforms import Cutout
 
 
 # fmt: on
 class CIFAR10DataModule(LightningDataModule):
+    """DataModule for CIFAR10.
+
+    Args:
+        root (str): Root directory of the datasets.
+        batch_size (int): Number of samples per batch.
+        val_split (float): Share of samples to use for validation. Defaults
+            to ``0.0``.
+        num_workers (int): Number of workers to use for data loading. Defaults
+            to ``1``.
+        cutout (int): Size of cutout to apply to images. Defaults to ``None``.
+        enable_randaugment (bool): Whether to apply RandAugment. Defaults to
+            ``False``.
+        auto_augment (str): Which auto-augment to apply. Defaults to ``None``.
+        test_alt (str): Which test set to use. Defaults to ``None``.
+        corruption_severity (int): Severity of corruption to apply for
+            CIFAR10-C. Defaults to ``1``.
+        num_dataloaders (int): Number of dataloaders to use. Defaults to ``1``.
+        pin_memory (bool): Whether to pin memory. Defaults to ``True``.
+        persistent_workers (bool): Whether to use persistent workers. Defaults
+            to ``True``.
+    """
+
     num_classes = 10
     num_channels = 3
     input_shape = (3, 32, 32)
+    training_task = "classification"
 
     def __init__(
         self,
         root: Union[str, Path],
+        ood_detection: bool,
         batch_size: int,
-        val_split: int = 0,
+        val_split: float = 0.0,
         num_workers: int = 1,
-        cutout: int = None,
-        auto_augment: str = None,
-        test_alt: str = None,
+        cutout: Optional[int] = None,
+        auto_augment: Optional[str] = None,
+        test_alt: Optional[Literal["c", "h"]] = None,
         corruption_severity: int = 1,
         num_dataloaders: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
         self.root: Path = root
+        self.ood_detection = ood_detection
         self.batch_size = batch_size
         self.val_split = val_split
         self.num_workers = num_workers
         self.num_dataloaders = num_dataloaders
 
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
@@ -101,27 +126,32 @@
             )
         else:
             self.dataset(
                 self.root,
                 download=True,
             )
 
-        self.ood_dataset(self.root, split="test", download=True)
+        if self.ood_detection:
+            self.ood_dataset(self.root, split="test", download=True)
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
             assert self.test_alt != "c", "CIFAR-C can only be used in testing."
             full = self.dataset(
                 self.root,
                 train=True,
                 download=False,
                 transform=self.transform_train,
             )
             self.train, self.val = random_split(
-                full, [len(full) - self.val_split, self.val_split]
+                full,
+                [
+                    int(len(full) * (1 - self.val_split)),
+                    len(full) - int(len(full) * (1 - self.val_split)),
+                ],
             )
             if self.val_split == 0:
                 self.val = self.dataset(
                     self.root,
                     train=False,
                     download=False,
                     transform=self.transform_test,
@@ -129,66 +159,76 @@
         elif stage == "test":
             self.test = self.dataset(
                 self.root,
                 train=False,
                 download=False,
                 transform=self.transform_test,
             )
-            self.ood = self.ood_dataset(
-                self.root,
-                split="test",
-                download=False,
-                transform=self.transform_test,
-            )
         else:
             self.test = self.dataset(
                 self.root,
                 severity=self.corruption_severity,
                 transform=self.transform_test,
             )
-
+        if self.ood_detection:
             self.ood = self.ood_dataset(
                 self.root,
                 split="test",
                 download=False,
                 transform=self.transform_test,
             )
 
     def train_dataloader(self) -> DataLoader:
-        r"""Gets the training dataloader for CIFAR10.
-        Returns:
+        r"""Get the training dataloader for CIFAR10.
+
+        Return:
             DataLoader: CIFAR10 training dataloader.
         """
         if self.num_dataloaders > 1:
             return self._data_loader(
                 AggregatedDataset(self.train, self.num_dataloaders),
                 shuffle=True,
             )
         else:
             return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
         r"""Gets the validation dataloader for CIFAR10.
+
         Returns:
             DataLoader: CIFAR10 validation dataloader.
         """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
-        r"""Gets the test dataloaders for CIFAR10.
-        Returns:
+        r"""Get the test dataloaders for CIFAR10.
+
+        Return:
             List[DataLoader]: Dataloaders of the CIFAR10 test set (in
                 distribution data) and SVHN test split (out-of-distribution
                 data).
         """
-        return [self._data_loader(self.test), self._data_loader(self.ood)]
+        dataloader = [self._data_loader(self.test)]
+        if self.ood_detection:
+            dataloader.append(self._data_loader(self.ood))
+        return dataloader
 
     def _data_loader(
         self, dataset: Dataset, shuffle: bool = False
     ) -> DataLoader:
+        """Create a dataloader for a given dataset.
+
+        Args:
+            dataset (Dataset): Dataset to create a dataloader for.
+            shuffle (bool, optional): Whether to shuffle the dataset. Defaults
+                to False.
+
+        Return:
+            DataLoader: Dataloader for the given dataset.
+        """
         return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=shuffle,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
             persistent_workers=self.persistent_workers,
@@ -199,16 +239,19 @@
         cls,
         parent_parser: ArgumentParser,
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
         p.add_argument("--batch_size", type=int, default=128)
-        p.add_argument("--val_split", type=int, default=0)
+        p.add_argument("--val_split", type=float, default=0.0)
         p.add_argument("--num_workers", type=int, default=4)
+        p.add_argument(
+            "--evaluate_ood", dest="ood_detection", action="store_true"
+        )
         p.add_argument("--cutout", type=int, default=0)
         p.add_argument("--auto_augment", type=str)
         p.add_argument("--test_alt", choices=["c", "h"], default=None)
         p.add_argument(
             "--severity", dest="corruption_severity", type=int, default=None
         )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/cifar100.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datamodules/cifar100.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # fmt: off
 from argparse import ArgumentParser
 from pathlib import Path
-from typing import Any, List, Optional, Union
+from typing import Any, List, Literal, Optional, Union
 
 import torch
 import torch.nn as nn
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
 from timm.data.auto_augment import rand_augment_transform
 from torch.utils.data import DataLoader, Dataset, random_split
@@ -13,40 +13,65 @@
 
 from ..datasets import CIFAR100_C, AggregatedDataset
 from ..transforms import Cutout
 
 
 # fmt: on
 class CIFAR100DataModule(LightningDataModule):
+    """DataModule for CIFAR100.
+
+    Args:
+        root (str): Root directory of the datasets.
+        batch_size (int): Number of samples per batch.
+        val_split (float): Share of samples to use for validation. Defaults
+            to ``0.0``.
+        num_workers (int): Number of workers to use for data loading. Defaults
+            to ``1``.
+        cutout (int): Size of cutout to apply to images. Defaults to ``None``.
+        enable_randaugment (bool): Whether to apply RandAugment. Defaults to
+            ``False``.
+        auto_augment (str): Which auto-augment to apply. Defaults to ``None``.
+        test_alt (str): Which test set to use. Defaults to ``None``.
+        corruption_severity (int): Severity of corruption to apply to
+            CIFAR100-C. Defaults to ``1``.
+        num_dataloaders (int): Number of dataloaders to use. Defaults to ``1``.
+        pin_memory (bool): Whether to pin memory. Defaults to ``True``.
+        persistent_workers (bool): Whether to use persistent workers. Defaults
+            to ``True``.
+    """
+
     num_classes = 100
     num_channels = 3
     input_shape = (3, 32, 32)
+    training_task = "classification"
 
     def __init__(
         self,
         root: Union[str, Path],
+        ood_detection: bool,
         batch_size: int,
-        val_split: int = 0,
+        val_split: float = 0.0,
         num_workers: int = 1,
-        cutout: int = None,
+        cutout: Optional[int] = None,
         enable_randaugment: bool = False,
-        auto_augment: str = None,
-        test_alt: str = None,
+        auto_augment: Optional[str] = None,
+        test_alt: Optional[Literal["c"]] = None,
         corruption_severity: int = 1,
         num_dataloaders: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
+        self.ood_detection = ood_detection
         self.batch_size = batch_size
         self.val_split = val_split
         self.num_workers = num_workers
         self.num_dataloaders = num_dataloaders
 
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
@@ -103,32 +128,37 @@
         )
 
     def prepare_data(self) -> None:
         if self.test_alt is None:
             self.dataset(self.root, train=True, download=True)
             self.dataset(self.root, train=False, download=True)
 
-        self.ood_dataset(
-            self.root,
-            split="test",
-            download=True,
-            transform=self.transform_test,
-        )
+        if self.ood_detection:
+            self.ood_dataset(
+                self.root,
+                split="test",
+                download=True,
+                transform=self.transform_test,
+            )
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
             assert self.test_alt != "c", "CIFAR-C can only be used in testing."
             full = self.dataset(
                 self.root,
                 train=True,
                 download=False,
                 transform=self.transform_train,
             )
             self.train, self.val = random_split(
-                full, [len(full) - self.val_split, self.val_split]
+                full,
+                [
+                    int(len(full) * (1 - self.val_split)),
+                    len(full) - int(len(full) * (1 - self.val_split)),
+                ],
             )
             if self.val_split == 0:
                 self.val = self.dataset(
                     self.root,
                     train=False,
                     download=False,
                     transform=self.transform_test,
@@ -143,53 +173,70 @@
                 )
             else:
                 self.test = self.dataset(
                     self.root,
                     transform=self.transform_test,
                     severity=self.corruption_severity,
                 )
-            self.ood = self.ood_dataset(
-                self.root,
-                split="test",
-                download=False,
-                transform=self.transform_test,
-            )
+            if self.ood_detection:
+                self.ood = self.ood_dataset(
+                    self.root,
+                    split="test",
+                    download=False,
+                    transform=self.transform_test,
+                )
 
     def train_dataloader(self) -> DataLoader:
-        r"""Gets the training dataloader for CIFAR100.
-        Returns:
+        """Get the training dataloader for CIFAR100.
+
+        Return:
             DataLoader: CIFAR100 training dataloader.
         """
         if self.num_dataloaders > 1:
             return self._data_loader(
                 AggregatedDataset(self.train, self.num_dataloaders),
                 shuffle=True,
             )
         else:
             return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
-        r"""Gets the validation dataloader for CIFAR100.
-        Returns:
+        """Get the validation dataloader for CIFAR100.
+
+        Return:
             DataLoader: CIFAR100 validation dataloader.
         """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
-        r"""Gets the test dataloaders for CIFAR100.
-        Returns:
+        """Get the test dataloaders for CIFAR100.
+
+        Return:
             List[DataLoader]: Dataloaders of the CIFAR100 test set (in
                 distribution data) and SVHN test split (out-of-distribution
                 data).
         """
-        return [self._data_loader(self.test), self._data_loader(self.ood)]
+        dataloader = [self._data_loader(self.test)]
+        if self.ood_detection:
+            dataloader.append(self._data_loader(self.ood))
+        return dataloader
 
     def _data_loader(
         self, dataset: Dataset, shuffle: bool = False
     ) -> DataLoader:
+        """Create a dataloader for a given dataset.
+
+        Args:
+            dataset (Dataset): Dataset to create a dataloader for.
+            shuffle (bool, optional): Whether to shuffle the dataset. Defaults
+                to False.
+
+        Return:
+            DataLoader: Dataloader for the given dataset.
+        """
         return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=shuffle,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
             persistent_workers=self.persistent_workers,
@@ -200,16 +247,19 @@
         cls,
         parent_parser: ArgumentParser,
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
         p.add_argument("--batch_size", type=int, default=128)
-        p.add_argument("--val_split", type=int, default=0)
+        p.add_argument("--val_split", type=float, default=0.0)
         p.add_argument("--num_workers", type=int, default=4)
+        p.add_argument(
+            "--evaluate_ood", dest="ood_detection", action="store_true"
+        )
         p.add_argument("--cutout", type=int, default=0)
         p.add_argument(
             "--randaugment", dest="enable_randaugment", action="store_true"
         )
         p.add_argument("--auto_augment", type=str)
         p.add_argument("--test_alt", choices=["c"], default=None)
         p.add_argument(
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/imagenet.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datamodules/imagenet.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,47 +3,51 @@
 from pathlib import Path
 from typing import Any, List, Optional, Union
 
 import torch.nn as nn
 import torchvision.transforms as T
 from pytorch_lightning import LightningDataModule
 from timm.data.auto_augment import rand_augment_transform
+from timm.data.mixup import Mixup
 from torch.utils.data import DataLoader, Dataset
 from torchvision.datasets import DTD, SVHN, ImageNet, INaturalist
 
 from ..datasets import ImageNetA, ImageNetO, ImageNetR
 
 
 # fmt: on
 class ImageNetDataModule(LightningDataModule):
     num_classes = 1000
     num_channels = 3
     test_datasets = ["r", "o", "a"]
     ood_datasets = ["inaturalist", "imagenet-o", "svhn", "textures"]
+    training_task = "classification"
 
     def __init__(
         self,
         root: Union[str, Path],
+        ood_detection: bool,
         batch_size: int,
         ood_ds: str = "svhn",
-        test_alt: str = None,
+        test_alt: Optional[str] = None,
         procedure: str = "A3",
         train_size: int = 224,
-        rand_augment_opt: str = None,
+        rand_augment_opt: Optional[str] = None,
         num_workers: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
+        self.ood_detection = ood_detection
         self.batch_size = batch_size
         self.num_workers = num_workers
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
         self.ood_ds = ood_ds
         self.test_alt = test_alt
 
@@ -72,14 +76,23 @@
         if self.procedure is None:
             print("Custom Procedure")
             train_size = train_size
             if rand_augment_opt is not None:
                 main_transform = rand_augment_transform(rand_augment_opt, {})
             else:
                 main_transform = nn.Identity()
+        elif self.procedure == "ViT":
+            train_size = 224
+            main_transform = T.Compose(
+                [
+                    Mixup(mixup_alpha=0.2, cutmix_alpha=1.0),
+                    rand_augment_transform("rand-m9-n2-mstd0.5", {}),
+                ]
+            )
+
         elif self.procedure == "A3":
             print("Procedure A3")
             train_size = 160
             main_transform = rand_augment_transform("rand-m6-mstd0.5-inc1", {})
         else:
             raise ValueError("The procedure is unknown")
 
@@ -109,38 +122,39 @@
                 f" make sure the folder contains a subfolder named {split}"
             )
 
     def prepare_data(self) -> None:
         if self.test_alt is not None:
             self.data = self.dataset(
                 self.root,
-                split="test",
-                download=True,
-            )
-        if self.ood_ds == "inaturalist":
-            self.ood = self.ood_dataset(
-                self.root,
-                version="2021_valid",
-                download=True,
-                transform=self.transform_test,
-            )
-        elif self.ood_ds != "textures":
-            self.ood = self.ood_dataset(
-                self.root,
-                split="test",
-                download=True,
-                transform=self.transform_test,
-            )
-        else:
-            self.ood = self.ood_dataset(
-                self.root,
-                split="train",
+                split="val",
                 download=True,
-                transform=self.transform_test,
             )
+        if self.ood_detection:
+            if self.ood_ds == "inaturalist":
+                self.ood = self.ood_dataset(
+                    self.root,
+                    version="2021_valid",
+                    download=True,
+                    transform=self.transform_test,
+                )
+            elif self.ood_ds != "textures":
+                self.ood = self.ood_dataset(
+                    self.root,
+                    split="test",
+                    download=True,
+                    transform=self.transform_test,
+                )
+            else:
+                self.ood = self.ood_dataset(
+                    self.root,
+                    split="train",
+                    download=True,
+                    transform=self.transform_test,
+                )
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
             if self.test_alt is not None:
                 raise ValueError(
                     "The test_alt argument is not supported for training."
                 )
@@ -156,52 +170,70 @@
             )
         if stage == "test":
             self.test = self.dataset(
                 self.root,
                 split="val",
                 transform=self.transform_test,
             )
+
+        if self.ood_detection:
             if self.ood_ds == "inaturalist":
                 self.ood = self.ood_dataset(
                     self.root,
                     version="2021_valid",
                     transform=self.transform_test,
                 )
             else:
                 self.ood = self.ood_dataset(
                     self.root,
                     transform=self.transform_test,
                     download=True,
                 )
 
     def train_dataloader(self) -> DataLoader:
-        r"""Gets the training dataloader for ImageNet.
-        Returns:
+        """Get the training dataloader for ImageNet.
+
+        Return:
             DataLoader: ImageNet training dataloader.
         """
         return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
-        r"""Gets the validation dataloader for ImageNet.
-        Returns:
+        """Get the validation dataloader for ImageNet.
+
+        Return:
             DataLoader: ImageNet validation dataloader.
         """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
-        r"""Gets test dataloaders for ImageNet.
-        Returns:
+        """Get the test dataloaders for ImageNet.
+
+        Return:
             List[DataLoader]: ImageNet test set (in distribution data) and
             Textures test split (out-of-distribution data).
         """
-        return [self._data_loader(self.test), self._data_loader(self.ood)]
+        dataloader = [self._data_loader(self.test)]
+        if self.ood_detection:
+            dataloader.append(self._data_loader(self.ood))
+        return dataloader
 
     def _data_loader(
         self, dataset: Dataset, shuffle: bool = False
     ) -> DataLoader:
+        """Create a dataloader for a given dataset.
+
+        Args:
+            dataset (Dataset): Dataset to create a dataloader for.
+            shuffle (bool, optional): Whether to shuffle the dataset. Defaults
+                to False.
+
+        Return:
+            DataLoader: Dataloader for the given dataset.
+        """
         return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=shuffle,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
             persistent_workers=self.persistent_workers,
@@ -213,15 +245,18 @@
         parent_parser: ArgumentParser,
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
         p.add_argument("--batch_size", type=int, default=256)
         p.add_argument("--num_workers", type=int, default=4)
+        p.add_argument(
+            "--evaluate_ood", dest="ood_detection", action="store_true"
+        )
         p.add_argument("--ood_ds", choices=cls.ood_datasets, default="svhn")
         p.add_argument("--test_alt", choices=cls.test_datasets, default=None)
-        p.add_argument("--procedure", choices=["A3"], default=None)
+        p.add_argument("--procedure", choices=["ViT", "A3"], default=None)
         p.add_argument("--train_size", type=int, default=224)
         p.add_argument(
             "--rand_augment", dest="rand_augment_opt", type=str, default=None
         )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/mnist.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datamodules/mnist.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,35 +10,53 @@
 from torchvision.datasets import MNIST, FashionMNIST
 
 from torch_uncertainty.transforms import Cutout
 
 
 # fmt: on
 class MNISTDataModule(LightningDataModule):
+    """DataModule for MNIST.
+
+    Args:
+        root (str): Root directory of the datasets.
+        batch_size (int): Number of samples per batch.
+        val_split (float): Share of samples to use for validation. Defaults
+            to ``0.0``.
+        num_workers (int): Number of workers to use for data loading. Defaults
+            to ``1``.
+        cutout (int): Size of cutout to apply to images. Defaults to ``None``.
+        pin_memory (bool): Whether to pin memory. Defaults to ``True``.
+        persistent_workers (bool): Whether to use persistent workers. Defaults
+            to ``True``.
+    """
+
     num_classes = 10
     num_channels = 1
     input_shape = (1, 28, 28)
+    training_task = "classification"
 
     def __init__(
         self,
         root: Union[str, Path],
+        ood_detection: bool,
         batch_size: int,
-        val_split: int = 0,
+        val_split: float = 0.0,
         num_workers: int = 1,
-        cutout: int = None,
+        cutout: Optional[int] = None,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
 
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
+        self.ood_detection = ood_detection
         self.batch_size = batch_size
         self.val_split = val_split
         self.num_workers = num_workers
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
         self.dataset = MNIST
         self.ood_dataset = FashionMNIST
@@ -62,28 +80,33 @@
                 T.ToTensor(),
                 T.CenterCrop(28),
                 T.Normalize((0.1307,), (0.3081,)),
             ]
         )
 
     def prepare_data(self) -> None:
+        """Download the datasets."""
         self.dataset(self.root, train=True, download=True)
         self.dataset(self.root, train=False, download=True)
         self.ood_dataset(self.root, download=True)
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
             full = self.dataset(
                 self.root,
                 train=True,
                 download=False,
                 transform=self.transform_train,
             )
             self.train, self.val = random_split(
-                full, [len(full) - self.val_split, self.val_split]
+                full,
+                [
+                    int(len(full) * (1 - self.val_split)),
+                    len(full) - int(len(full) * (1 - self.val_split)),
+                ],
             )
             if self.val_split == 0:
                 self.val = self.dataset(
                     self.root,
                     train=False,
                     download=False,
                     transform=self.transform_test,
@@ -91,46 +114,64 @@
         if stage == "test":
             self.test = self.dataset(
                 self.root,
                 train=False,
                 download=False,
                 transform=self.transform_test,
             )
+
+        if self.ood_detection:
             self.ood = self.ood_dataset(
                 self.root,
                 download=False,
                 transform=self.transform_test,
             )
 
     def train_dataloader(self) -> DataLoader:
-        r"""Gets the training dataloader for MNIST.
-        Returns:
+        r"""Get the training dataloader for MNIST.
+
+        Return:
             DataLoader: MNIST training dataloader.
         """
         return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
-        r"""Gets the validation dataloader for MNIST.
-        Returns:
+        r"""Get the validation dataloader for MNIST.
+
+        Return:
             DataLoader: MNIST validation dataloader.
         """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
-        r"""Gets the test dataloaders for MNIST.
-        Returns:
+        r"""Get the test dataloaders for MNIST.
+
+        Return:
             List[DataLoader]: Dataloaders of the MNIST test set (in
                 distribution data) and FashionMNIST test split
                 (out-of-distribution data).
         """
-        return [self._data_loader(self.test), self._data_loader(self.ood)]
+        dataloader = [self._data_loader(self.test)]
+        if self.ood_detection:
+            dataloader.append(self._data_loader(self.ood))
+        return dataloader
 
     def _data_loader(
         self, dataset: Dataset, shuffle: bool = False
     ) -> DataLoader:
+        """Create a dataloader for a given dataset.
+
+        Args:
+            dataset (Dataset): Dataset to create a dataloader for.
+            shuffle (bool, optional): Whether to shuffle the dataset. Defaults
+                to False.
+
+        Return:
+            DataLoader: Dataloader for the given dataset.
+        """
         return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=shuffle,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
             persistent_workers=self.persistent_workers,
@@ -143,8 +184,11 @@
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
         p.add_argument("--batch_size", type=int, default=128)
         p.add_argument("--val_split", type=int, default=0)
         p.add_argument("--num_workers", type=int, default=4)
+        p.add_argument(
+            "--evaluate_ood", dest="ood_detection", action="store_true"
+        )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datamodules/tiny_imagenet.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datamodules/tiny_imagenet.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,34 @@
 from ..datasets import TinyImageNet
 
 
 # fmt: on
 class TinyImageNetDataModule(LightningDataModule):
     num_classes = 200
     num_channels = 3
+    training_task = "classification"
 
     def __init__(
         self,
         root: Union[str, Path],
+        ood_detection: bool,
         batch_size: int,
-        rand_augment_opt: str = None,
+        rand_augment_opt: Optional[str] = None,
         num_workers: int = 1,
         pin_memory: bool = True,
         persistent_workers: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
         # TODO: COMPUTE STATS
         if isinstance(root, str):
             root = Path(root)
 
         self.root: Path = root
+        self.ood_detection = ood_detection
         self.batch_size = batch_size
         self.num_workers = num_workers
         self.pin_memory = pin_memory
         self.persistent_workers = persistent_workers
         self.dataset = TinyImageNet
         self.ood_dataset = SVHN
 
@@ -68,15 +71,16 @@
         if split not in list(self.root.iterdir()):
             raise FileNotFoundError(
                 f"a {split} TinyImagenet split was not found in {self.root},"
                 f" make sure the folder contains a subfolder named {split}"
             )
 
     def prepare_data(self) -> None:
-        self.ood_dataset(self.root, split="test", download=True)
+        if self.ood_detection:
+            self.ood_dataset(self.root, split="test", download=True)
 
     def setup(self, stage: Optional[str] = None) -> None:
         if stage == "fit" or stage is None:
             self.train = self.dataset(
                 self.root,
                 split="train",
                 transform=self.transform_train,
@@ -88,45 +92,63 @@
             )
         if stage == "test":
             self.test = self.dataset(
                 self.root,
                 split="val",
                 transform=self.transform_test,
             )
+
+        if self.ood_detection:
             self.ood = self.ood_dataset(
                 self.root,
                 split="test",
                 transform=self.transform_test,
             )
 
     def train_dataloader(self) -> DataLoader:
-        r"""Gets the training dataloader for TinyImageNet.
-        Returns:
+        r"""Get the training dataloader for TinyImageNet.
+
+        Return:
             DataLoader: TinyImageNet training dataloader.
         """
         return self._data_loader(self.train, shuffle=True)
 
     def val_dataloader(self) -> DataLoader:
-        r"""Gets the validation dataloader for TinyImageNet.
-        Returns:
+        r"""Get the validation dataloader for TinyImageNet.
+
+        Return:
             DataLoader: TinyImageNet validation dataloader.
         """
         return self._data_loader(self.val)
 
     def test_dataloader(self) -> List[DataLoader]:
-        r"""Gets test dataloaders for TinyImageNet.
-        Returns:
+        r"""Get test dataloaders for TinyImageNet.
+
+        Return:
             List[DataLoader]: TinyImageNet test set (in distribution data) and
             SVHN test split (out-of-distribution data).
         """
-        return [self._data_loader(self.test), self._data_loader(self.ood)]
+        dataloader = [self._data_loader(self.test)]
+        if self.ood_detection:
+            dataloader.append(self._data_loader(self.ood))
+        return dataloader
 
     def _data_loader(
         self, dataset: Dataset, shuffle: bool = False
     ) -> DataLoader:
+        """Create a dataloader for a given dataset.
+
+        Args:
+            dataset (Dataset): Dataset to create a dataloader for.
+            shuffle (bool, optional): Whether to shuffle the dataset. Defaults
+                to False.
+
+        Return:
+            DataLoader: Dataloader for the given dataset.
+        """
         return DataLoader(
             dataset,
             batch_size=self.batch_size,
             shuffle=shuffle,
             num_workers=self.num_workers,
             pin_memory=self.pin_memory,
             persistent_workers=self.persistent_workers,
@@ -139,10 +161,13 @@
         **kwargs: Any,
     ) -> ArgumentParser:
         p = parent_parser.add_argument_group("datamodule")
         p.add_argument("--root", type=str, default="./data/")
         p.add_argument("--batch_size", type=int, default=256)
         p.add_argument("--num_workers", type=int, default=4)
         p.add_argument(
+            "--evaluate_ood", dest="ood_detection", action="store_true"
+        )
+        p.add_argument(
             "--rand_augment", dest="rand_augment_opt", type=str, default=None
         )
         return parent_parser
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datasets/aggregated_dataset.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datasets/aggregated_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class AggregatedDataset(Dataset):
     def __init__(self, dataset: Dataset, n_dataloaders: int) -> None:
         super().__init__()
         self.dataset = dataset
         self.n_dataloaders = n_dataloaders
-        self.dataset_size = len(self.dataset)
+        self.dataset_size = len(dataset)
         self.offset = self.dataset_size // self.n_dataloaders
 
     def __getitem__(self, idx: int):
         inputs, targets = zip(
             *[
                 self.dataset[(idx + i * self.offset) % self.dataset_size]
                 for i in range(self.n_dataloaders)
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/cifar_c.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datasets/cifar/cifar_c.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,36 @@
 
 import numpy as np
 
 # fmt:on
 
 
 class CIFAR10_C(VisionDataset):
+    """The corrupted CIFAR-10-C Dataset.
+
+    Args:
+        root (str): Root directory of the datasets.
+        transform (callable, optional): A function/transform that takes in
+            a PIL image and returns a transformed version. E.g,
+            ``transforms.RandomCrop``. Defaults to None.
+        target_transform (callable, optional): A function/transform that
+            takes in the target and transforms it. Defaults to None.
+        subset (str): The subset to use, one of ``all`` or the keys in
+            ``cifarc_subsets``.
+        severity (int): The severity of the corruption, between 1 and 5.
+        download (bool, optional): If True, downloads the dataset from the
+            internet and puts it in root directory. If dataset is already
+            downloaded, it is not downloaded again. Defaults to False.
+
+    References:
+        Benchmarking neural network robustness to common corruptions and
+            perturbations. Dan Hendrycks and Thomas Dietterich.
+            In ICLR, 2019.
+    """
+
     base_folder = "CIFAR-10-C"
     tgz_md5 = "56bf5dcef84df0e2308c6dcbcbbd8499"
     cifarc_subsets = [
         "brightness",
         "contrast",
         "defocus_blur",
         "elastic_transform",
@@ -142,14 +164,15 @@
             ]
             labels: np.ndarray = np.load(root / "labels.npy")[
                 (severity - 1) * 10000 : severity * 10000
             ]
         return samples, labels
 
     def __len__(self) -> int:
+        """The number of samples in the dataset."""
         return self.labels.shape[0]
 
     def __getitem__(self, index: int) -> Any:
         sample, target = (
             self.samples[index],
             self.labels[index],
         )
@@ -157,21 +180,23 @@
         if self.transform is not None:
             sample = self.transform(sample)
         if self.target_transform is not None:
             target = self.target_transform(target)
         return sample, target
 
     def _check_integrity(self) -> bool:
+        """Check the integrity of the dataset."""
         for filename, md5 in self.ctest_list:
             fpath = os.path.join(self.root, self.base_folder, filename)
             if not check_integrity(fpath, md5):
                 return False
         return True
 
     def download(self) -> None:
+        """Download the dataset."""
         if self._check_integrity():
             print("Files already downloaded and verified.")
             return
         download_and_extract_archive(
             self.url, self.root, filename=self.filename, md5=self.tgz_md5
         )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datasets/cifar/cifar_h.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datasets/cifar/cifar_h.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 # fmt:off
 import os
-from typing import Any, Callable
+from typing import Any, Callable, Optional
 
 import torch
 from torchvision.datasets import CIFAR10
 from torchvision.datasets.utils import check_integrity, download_url
 
 import numpy as np
 
 
 # fmt:on
 class CIFAR10_H(CIFAR10):
-    htest_list = [["cifar-10h-probs.npy", "7b41f73eee90fdefc73bfc820ab29ba8"]]
-    url = (
+    """`CIFAR-10H <https://github.com/jcpeterson/cifar-10h>`_ Dataset.
+
+    Args:
+        root (string): Root directory of dataset where file
+            ``cifar-10h-probs.npy`` exists or will be saved to if download
+            is set to True.
+        train (bool, optional): For API consistency, not used.
+        transform (callable, optional): A function/transform that takes in
+            a PIL image and returns a transformed version. E.g,
+            ``transforms.RandomCrop``. Defaults to None.
+        target_transform (callable, optional): A function/transform that
+            takes in the target and transforms it. Defaults to None.
+        download (bool, optional): If True, downloads the dataset from the
+            internet and puts it in root directory. If dataset is already
+            downloaded, it is not downloaded again. Defaults to False.
+    """
+
+    h_test_list = ["cifar-10h-probs.npy", "7b41f73eee90fdefc73bfc820ab29ba8"]
+    h_url = (
         "https://github.com/jcpeterson/cifar-10h/raw/master/data/"
         "cifar10h-probs.npy"
     )
 
     def __init__(
         self,
         root: str,
-        train: bool = None,
-        transform: Callable[..., Any] = None,
-        target_transform: Callable[..., Any] = None,
+        train: Optional[bool] = None,
+        transform: Optional[Callable[..., Any]] = None,
+        target_transform: Optional[Callable[..., Any]] = None,
         download: bool = False,
     ) -> None:
-        """`CIFAR-10H <https://github.com/jcpeterson/cifar-10h>`_ Dataset.
-
-        Args:
-            root (string): Root directory of dataset where file
-                ``cifar-10h-probs.npy`` exists or will be saved to if download
-                is set to True.
-            train (bool, optional): For API consistency, not used.
-            transform (callable, optional): A function/transform that takes in
-                a PIL image and returns a transformed version. E.g,
-                ``transforms.RandomCrop``
-            target_transform (callable, optional): A function/transform that
-                takes in the target and transforms it.
-            download (bool, optional): If True, downloads the dataset from the
-                internet and puts it in root directory. If dataset is already
-                downloaded, it is not downloaded again.
-        """
-
+        if train:
+            raise ValueError("CIFAR10_H does not support training data.")
         print(
             "WARNING: CIFAR10_H cannot be used with Classification routines "
             "for now."
         )
         super().__init__(
             root,
             train=False,
             transform=transform,
             target_transform=target_transform,
             download=download,
         )
 
         if download:
-            self.download()
+            self.download_h()
 
         if not self._check_specific_integrity():
             raise RuntimeError(
                 "Dataset not found or corrupted. You can use download=True to "
                 "download it."
             )
 
         self.targets = list(
             torch.as_tensor(
-                np.load(os.path.join(self.root, self.htest_list[0][0]))
+                np.load(os.path.join(self.root, self.h_test_list[0]))
             )
         )
 
     def _check_specific_integrity(self) -> bool:
-        for filename, md5 in self.htest_list:
-            fpath = os.path.join(self.root, filename)
-            if not check_integrity(fpath, md5):
-                return False
+        filename, md5 = self.h_test_list
+        fpath = os.path.join(self.root, filename)
+        if not check_integrity(fpath, md5):
+            return False
         return True
 
-    def download(self) -> None:
+    def download_h(self) -> None:
         download_url(
-            self.url,
+            self.h_url,
             self.root,
-            filename=self.htest_list[0][0],
-            md5=self.htest_list[0][1],
+            filename=self.h_test_list[0],
+            md5=self.h_test_list[1],
         )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/datasets/fractals.py` & `torch_uncertainty-0.1.3/torch_uncertainty/datasets/fractals.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # fmt: off
 from pathlib import Path
-from typing import Any, Callable, Tuple
+from typing import Any, Callable, Optional, Tuple
 
 from torchvision.datasets import ImageFolder
 from torchvision.datasets.utils import (
     check_integrity,
     download_file_from_google_drive,
     extract_archive,
 )
 
 
 # fmt: on
 class Fractals(ImageFolder):
+    """Dataset used for PixMix augmentations.
+
+    Args:
+        root (str): Root directory of dataset.
+
+    Note:
+        There is no information on the license of the dataset. It may not
+        be suitable for commercial use.
+    """
+
     file_id = "1qC2gIUx9ARU7zhgI4IwGD3YcFhm8J4cA"
     filename = "fractals_and_fvis.tar"
     tgz_md5 = "3619fb7e2c76130749d97913fdd3ab27"
 
     def __init__(
         self,
         root: str,
-        transform: Callable[..., Any] = None,
-        target_transform: Callable[..., Any] = None,
+        transform: Optional[Callable[..., Any]] = None,
+        target_transform: Optional[Callable[..., Any]] = None,
         download: bool = False,
     ):
-        """Dataset used for PixMix augmentations.
-
-        Args:
-            root (str): Root directory of dataset.
-
-        Note:
-            There is no information on the license of the dataset. It may not
-            be suitable for commercial use.
-        """
-
         if isinstance(root, str):
             self.root = Path(root)
 
         if download:
             self.download()
 
         if not self._check_integrity():
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/layers/batchens_layers.py` & `torch_uncertainty-0.1.3/torch_uncertainty/layers/batchens_layers.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/layers/masksembles_layers.py` & `torch_uncertainty-0.1.3/torch_uncertainty/layers/masksembles_layers.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/layers/packed_layers.py` & `torch_uncertainty-0.1.3/torch_uncertainty/layers/packed_layers.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,46 @@
 import torch.nn as nn
 from einops import rearrange
 from torch import Tensor
 from torch.nn.common_types import _size_2_t
 
 
 # fmt: on
+def check_packed_parameters_consistency(
+    alpha: float, num_estimators: int, gamma: int
+) -> None:
+    if alpha is None:
+        raise ValueError("You must specify the value of the arg. `alpha`")
+
+    if alpha <= 0:
+        raise ValueError(f"Attribute `alpha` should be > 0, not {alpha}")
+
+    if num_estimators is None:
+        raise ValueError(
+            "You must specify the value of the arg. `num_estimators`"
+        )
+    if not isinstance(num_estimators, int):
+        raise ValueError(
+            "Attribute `num_estimators` should be an int, not "
+            f"{type(num_estimators)}"
+        )
+    if num_estimators <= 0:
+        raise ValueError(
+            "Attribute `num_estimators` should be >= 1, not "
+            f"{num_estimators}"
+        )
+
+    if not isinstance(gamma, int):
+        raise ValueError(
+            f"Attribute `gamma` should be an int, not " f"{type(gamma)}"
+        )
+    if gamma <= 0:
+        raise ValueError(f"Attribute `gamma` should be >= 1, not {gamma}")
+
+
 class PackedLinear(nn.Module):
     r"""Packed-Ensembles-style Linear layer.
 
     This layer computes fully-connected operation for a given number of
     estimators (:attr:`num_estimators`) using a `1x1` convolution.
 
     Args:
@@ -23,14 +55,20 @@
         bias (bool, optional): It ``True``, adds a learnable bias to the
             output. Defaults to ``True``.
         groups (int, optional): Number of blocked connections from input
             channels to output channels. Defaults to ``1``.
         rearrange (bool, optional): Rearrange the input and outputs for
             compatibility with previous and later layers. Defaults to ``True``.
 
+    Explanation Note:
+        Increasing :attr:`alpha` will increase the number of channels of the
+        ensemble, increasing its representation capacity. Increasing
+        :attr:`gamma` will increase the number of groups in the network and
+        therefore reduce the number of parameters.
+
     Note:
         Each ensemble member will only see
         :math:`\frac{\text{in_features}}{\text{num_estimators}}` features,
         so when using :attr:`groups` you should make sure that
         :attr:`in_features` and :attr:`out_features` are both divisible by
         :attr:`n_estimators` :math:`\times`:attr:`groups`. However, the
         number of input and output features will be changed to comply with
@@ -46,82 +84,104 @@
         self,
         in_features: int,
         out_features: int,
         alpha: float,
         num_estimators: int,
         gamma: int = 1,
         bias: bool = True,
-        groups: int = 1,
         rearrange: bool = True,
         first: bool = False,
         last: bool = False,
         device=None,
         dtype=None,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
 
-        if alpha <= 0:
-            raise ValueError(f"Attribute `alpha` should be > 0, not {alpha}")
-
-        if not isinstance(gamma, int):
-            raise ValueError(
-                f"Attribute `gamma` should be an int, not " f"{type(gamma)}"
-            )
-        if gamma <= 0:
-            raise ValueError(f"Attribute `gamma` should be >= 1, not {gamma}")
+        check_packed_parameters_consistency(alpha, num_estimators, gamma)
 
+        self.first = first
         self.num_estimators = num_estimators
         self.rearrange = rearrange
 
         # Define the number of features of the underlying convolution
         extended_in_features = int(in_features * (1 if first else alpha))
         extended_out_features = int(
             out_features * (num_estimators if last else alpha)
         )
 
         # Define the number of groups of the underlying convolution
-        actual_groups = num_estimators * gamma * groups
+        actual_groups = num_estimators * gamma if not first else 1
 
         # fix if not divisible by groups
         if extended_in_features % actual_groups:
             extended_in_features += num_estimators - extended_in_features % (
                 actual_groups
             )
         if extended_out_features % actual_groups:
             extended_out_features += num_estimators - extended_out_features % (
                 actual_groups
             )
 
-        self.conv1x1 = nn.Conv2d(
+        self.conv1x1 = nn.Conv1d(
             in_channels=extended_in_features,
             out_channels=extended_out_features,
             kernel_size=1,
             stride=1,
             padding=0,
             dilation=1,
             groups=actual_groups,
             bias=bias,
             padding_mode="zeros",
             **factory_kwargs,
         )
 
     def _rearrange_forward(self, x: Tensor) -> Tensor:
-        x = x.unsqueeze(-1).unsqueeze(-1)
-        x = rearrange(x, "(m e) c h w -> e (m c) h w", m=self.num_estimators)
+        x = x.unsqueeze(-1)
+        if not self.first:
+            x = rearrange(x, "(m e) c h -> e (m c) h", m=self.num_estimators)
+
         x = self.conv1x1(x)
-        x = rearrange(x, "e (m c) h w -> (m e) c h w", m=self.num_estimators)
-        return x.squeeze(-1).squeeze(-1)
+        x = rearrange(x, "e (m c) h -> (m e) c h", m=self.num_estimators)
+        return x.squeeze(-1)
 
     def forward(self, input: Tensor) -> Tensor:
         if self.rearrange:
             return self._rearrange_forward(input)
         else:
             return self.conv1x1(input)
 
+    @property
+    def weight(self) -> Tensor:
+        r"""The weight of the underlying convolutional layer."""
+        return self.conv1x1.weight
+
+    @property
+    def bias(self) -> Union[Tensor, None]:
+        r"""The bias of the underlying convolutional layer."""
+        return self.conv1x1.bias
+
+
+class PackedConv1d(nn.Module):
+    r"""Packed-Ensembles-style Conv1d layer.
+
+    Warning:
+        Not yet implemented (open an issue if desired).
+    """
+
+    def __init__(self, **kwargs) -> None:
+        raise NotImplementedError(
+            "Open an issue if you would like this layer to be implemented."
+        )
+
+    def forward(self, input: Tensor) -> Tensor:
+        raise NotImplementedError(
+            "Open an issue if you would like this layer to be implemented."
+        )
+
 
 class PackedConv2d(nn.Module):
     r"""Packed-Ensembles-style Conv2d layer.
 
     Args:
         in_channels (int): Number of channels in the input image.
         out_channels (int): Number of channels produced by the convolution.
@@ -138,14 +198,20 @@
         groups (int, optional): Number of blocked connexions from input
             channels to output channels for each estimator. Defaults to ``1``.
         minimum_channels_per_group (int, optional): Smallest possible number of
             hannels per group.
         bias (bool, optional): If ``True``, adds a learnable bias to the
             output. Defaults to ``True``.
 
+    Explanation Note:
+        Increasing :attr:`alpha` will increase the number of channels of the
+        ensemble, increasing its representation capacity. Increasing
+        :attr:`gamma` will increase the number of groups in the network and
+        therefore reduce the number of parameters.
+
     Note:
         Each ensemble member will only see
         :math:`\frac{\text{in_channels}}{\text{num_estimators}}` channels,
         so when using :attr:`groups` you should make sure that
         :attr:`in_channels` and :attr:`out_channels` are both divisible by
         :attr:`num_estimators` :math:`\times`:attr:`gamma` :math:`\times`
         :attr:`groups`. However, the number of input and output channels will
@@ -170,23 +236,15 @@
         last: bool = False,
         device: Union[Any, None] = None,
         dtype: Union[Any, None] = None,
     ) -> None:
         factory_kwargs = {"device": device, "dtype": dtype}
         super().__init__()
 
-        if alpha <= 0:
-            raise ValueError(f"Attribute `alpha` should be > 0, not {alpha}")
-
-        if not isinstance(gamma, int):
-            raise ValueError(
-                f"Attribute `gamma` should be an int, not " f"{type(gamma)}"
-            )
-        if gamma <= 0:
-            raise ValueError(f"Attribute `gamma` should be >= 1, not {gamma}")
+        check_packed_parameters_consistency(alpha, num_estimators, gamma)
 
         self.num_estimators = num_estimators
 
         # Define the number of channels of the underlying convolution
         extended_in_channels = int(in_channels * (1 if first else alpha))
         extended_out_channels = int(
             out_channels * (num_estimators if last else alpha)
@@ -225,14 +283,24 @@
             padding_mode="zeros",
             **factory_kwargs,
         )
 
     def forward(self, input: Tensor) -> Tensor:
         return self.conv(input)
 
+    @property
+    def weight(self) -> Tensor:
+        r"""The weight of the underlying convolutional layer."""
+        return self.conv.weight
+
+    @property
+    def bias(self) -> Union[Tensor, None]:
+        r"""The bias of the underlying convolutional layer."""
+        return self.conv.bias
+
 
 class PackedConv3d(nn.Module):
     r"""Packed-Ensembles-style Conv3d layer.
 
     Warning:
         Not yet implemented (open an issue if desired).
     """
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/metrics/brier_score.py` & `torch_uncertainty-0.1.3/torch_uncertainty/metrics/brier_score.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,27 +77,34 @@
 
     def update(self, probs: torch.Tensor, target: torch.Tensor) -> None:
         """
         Update the current Brier score with a new tensor of probabilities.
 
         Args:
             probs (torch.Tensor): A probability tensor of shape
-                (num_estimators, batch, num_classes) or
+                (batch, num_estimators, num_classes) or
                 (batch, num_classes)
         """
-        if len(target.shape) == 1:
+        if target.ndim == 1:
             target = F.one_hot(target, self.num_classes)
 
-        print("target", target.shape, "probs", probs.shape)
-        if len(probs.shape) == 2:
+        if self.num_classes == 1:
+            probs = probs.unsqueeze(-1)
+
+        if probs.ndim == 2:
             batch_size = probs.size(0)
-        else:
+        elif probs.ndim == 3:
             batch_size = probs.size(0)
             self.num_estimators = probs.size(1)
             target = target.unsqueeze(1).repeat(1, self.num_estimators, 1)
+        else:
+            raise ValueError(
+                f"Expected `probs` to be of shape (batch, num_classes) or "
+                f"(batch, num_estimators, num_classes) but got {probs.shape}"
+            )
 
         brier_score = F.mse_loss(probs, target, reduction="none").sum(dim=-1)
 
         if self.reduction is None or self.reduction == "none":
             self.values.append(brier_score)
         else:
             self.values += brier_score.sum()
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/metrics/disagreement.py` & `torch_uncertainty-0.1.3/torch_uncertainty/metrics/disagreement.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/metrics/entropy.py` & `torch_uncertainty-0.1.3/torch_uncertainty/metrics/entropy.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/metrics/fpr95.py` & `torch_uncertainty-0.1.3/torch_uncertainty/metrics/fpr95.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     rtol : float
         Relative tolerance, see ``np.allclose``
     atol : float
         Absolute tolerance, see ``np.allclose``
     """
     out = np.cumsum(arr, dtype=np.float64)
     expected = np.sum(arr, dtype=np.float64)
-    if not np.allclose(out[-1], expected, rtol=rtol, atol=atol):
+    if not np.allclose(
+        out[-1], expected, rtol=rtol, atol=atol
+    ):  # coverage: ignore
         raise RuntimeError(
             "cumsum was found to be unstable: "
             "its last element does not correspond to sum"
         )
     return out
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/metrics/jensen_shannon_divergence.py` & `torch_uncertainty-0.1.3/torch_uncertainty/metrics/jensen_shannon_divergence.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/metrics/mutual_information.py` & `torch_uncertainty-0.1.3/torch_uncertainty/metrics/mutual_information.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/metrics/nll.py` & `torch_uncertainty-0.1.3/torch_uncertainty/metrics/nll.py`

 * *Files 25% similar despite different names*

```diff
@@ -90,7 +90,56 @@
 
         if self.reduction == "sum":
             return values.sum(dim=-1)
         elif self.reduction == "mean":
             return values.sum(dim=-1) / self.total
         else:  # reduction is None or "none"
             return values
+
+
+class GaussianNegativeLogLikelihood(NegativeLogLikelihood):
+    """The Gaussian Negative Log Likelihood Metric.
+
+    Args:
+        reduction (str, optional): Determines how to reduce over the
+            :math:`B`/batch dimension:
+
+            - ``'mean'`` [default]: Averages score across samples
+            - ``'sum'``: Sum score across samples
+            - ``'none'`` or ``None``: Returns score per sample
+
+        kwargs: Additional keyword arguments, see `Advanced metric settings
+            <https://torchmetrics.readthedocs.io/en/stable/pages/overview.html#metric-kwargs>`_.
+
+    Inputs:
+        - :attr:`mean`: :math:`(B, D)`
+        - :attr:`target`: :math:`(B, D)`
+        - :attr:`var`: :math:`(B, D)`
+
+        where :math:`B` is the batch size and :math:`D` is the number of
+        dimensions. :math:`D` is optional.
+
+    Raises:
+        ValueError:
+            If :attr:`reduction` is not one of ``'mean'``, ``'sum'``,
+            ``'none'`` or ``None``.
+    """
+
+    def update(
+        self, mean: torch.Tensor, target: torch.Tensor, var: torch.Tensor
+    ) -> None:
+        """Update state with prediction mean, targets, and prediction varoance.
+
+        Args:
+            mean (torch.Tensor): Probabilities from the model.
+            target (torch.Tensor): Ground truth labels.
+            var (torch.Tensor): Predicted variance from the model.
+        """
+        if self.reduction is None or self.reduction == "none":
+            self.values.append(
+                F.gaussian_nll_loss(mean, target, var, reduction="none")
+            )
+        else:
+            self.values += F.gaussian_nll_loss(
+                mean, target, var, reduction="sum"
+            )
+            self.total += target.size(0)
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/metrics/variation_ratio.py` & `torch_uncertainty-0.1.3/torch_uncertainty/metrics/variation_ratio.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,9 +74,11 @@
                 / n_estimators
             )
 
         if self.reduction == "mean":
             variation_ratio = variation_ratio.mean()
         elif self.reduction == "sum":
             variation_ratio = variation_ratio.sum()
+        else:  # None
+            pass
 
         return variation_ratio
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/batched.py` & `torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/batched.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,22 +152,22 @@
         block: Type[Union[BasicBlock, Bottleneck]],
         num_blocks: List[int],
         in_channels: int,
         num_estimators: int,
         groups: int = 1,
         num_classes=10,
         width_multiplier: int = 1,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
     ):
         super().__init__()
         self.in_planes = 64 * width_multiplier
         self.num_estimators = num_estimators
 
         self.width_multiplier = width_multiplier
-        if imagenet_structure:
+        if style == "imagenet":
             self.conv1 = BatchConv2d(
                 3,
                 64 * self.width_multiplier,
                 kernel_size=7,
                 stride=2,
                 padding=3,
                 num_estimators=num_estimators,
@@ -183,15 +183,15 @@
                 padding=1,
                 num_estimators=num_estimators,
                 groups=groups,
                 bias=False,
             )
         self.bn1 = nn.BatchNorm2d(64 * self.width_multiplier)
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
             self.optional_pool = nn.Identity()
 
         self.layer1 = self._make_layer(
@@ -268,15 +268,15 @@
 
 
 def batched_resnet18(
     in_channels: int,
     num_estimators: int,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-18 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -289,24 +289,24 @@
     return _BatchedResNet(
         BasicBlock,
         [2, 2, 2, 2],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def batched_resnet34(
     in_channels: int,
     num_estimators: int,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-34 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -319,25 +319,25 @@
     return _BatchedResNet(
         BasicBlock,
         [3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def batched_resnet50(
     in_channels: int,
     num_estimators: int,
     groups: int,
     num_classes: int,
     width_multiplier: int = 1,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-50 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -351,24 +351,24 @@
         Bottleneck,
         [3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
         width_multiplier=width_multiplier,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def batched_resnet101(
     in_channels: int,
     num_estimators: int,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-101 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -381,41 +381,41 @@
     return _BatchedResNet(
         Bottleneck,
         [3, 4, 23, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def batched_resnet152(
     in_channels: int,
     num_estimators: int,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _BatchedResNet:
     """BatchEnsemble of ResNet-152 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         groups (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _BatchedResNet: A BatchEnsemble-style ResNet-152.
     """
     return _BatchedResNet(
         Bottleneck,
         [3, 8, 36, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         num_classes=num_classes,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/masked.py` & `torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/masked.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,28 +158,28 @@
         block: Type[Union[BasicBlock, Bottleneck]],
         num_blocks: List[int],
         in_channels: int,
         num_classes: int,
         num_estimators: int,
         scale: float = 2.0,
         groups: int = 1,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
     ) -> None:
         super().__init__()
 
         self.in_channels = in_channels
         self.num_estimators = num_estimators
         self.in_planes = 64
         if self.in_planes % self.num_estimators:
             self.in_planes += (
                 self.num_estimators - self.in_planes % self.num_estimators
             )
         block_planes = self.in_planes
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.conv1 = nn.Conv2d(
                 self.in_channels,
                 block_planes,
                 kernel_size=7,
                 stride=2,
                 padding=3,
                 groups=groups,
@@ -194,15 +194,15 @@
                 padding=1,
                 groups=groups,
                 bias=False,
             )
 
         self.bn1 = nn.BatchNorm2d(block_planes)
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
             self.optional_pool = nn.Identity()
 
         self.layer1 = self._make_layer(
@@ -295,15 +295,15 @@
 
 def masked_resnet18(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _MaskedResNet:
     """Masksembles of ResNet-18 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -317,25 +317,25 @@
         block=BasicBlock,
         num_blocks=[2, 2, 2, 2],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def masked_resnet34(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _MaskedResNet:
     """Masksembles of ResNet-34 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -349,25 +349,25 @@
         block=BasicBlock,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def masked_resnet50(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _MaskedResNet:
     """Masksembles of ResNet-50 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -381,25 +381,25 @@
         block=Bottleneck,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def masked_resnet101(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _MaskedResNet:
     """Masksembles of ResNet-101 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -413,25 +413,25 @@
         block=Bottleneck,
         num_blocks=[3, 4, 23, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def masked_resnet152(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _MaskedResNet:
     """Masksembles of ResNet-152 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
@@ -446,9 +446,9 @@
         block=Bottleneck,
         num_blocks=[3, 8, 36, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/packed.py` & `torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/packed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # fmt: off
-from typing import List, Type, Union
+from typing import Any, Dict, List, Type, Union
 
 import torch.nn as nn
 import torch.nn.functional as F
 from einops import rearrange
 from torch import Tensor
 
 from ...layers import PackedConv2d, PackedLinear
@@ -16,41 +16,34 @@
     "packed_resnet50",
     "packed_resnet101",
     "packed_resnet152",
 ]
 
 weight_ids = {
     "10": {
-        "18": None,
+        "18": "pe_resnet18_c10",
         "32": None,
         "50": "pe_resnet50_c10",
         "101": None,
         "152": None,
     },
     "100": {
-        "18": None,
+        "18": "pe_resnet18_c100",
         "32": None,
         "50": "pe_resnet50_c100",
         "101": None,
         "152": None,
     },
     "1000": {
         "18": None,
         "32": None,
         "50": "pe_resnet50_in1k",
         "101": None,
         "152": None,
     },
-    "1000_wider": {
-        "18": None,
-        "32": None,
-        "50": "pex4_resnet50",
-        "101": None,
-        "152": None,
-    },
 }
 
 
 class BasicBlock(nn.Module):
     expansion = 1
 
     def __init__(
@@ -202,24 +195,27 @@
         num_blocks: List[int],
         in_channels: int,
         num_classes: int,
         num_estimators: int,
         alpha: int = 2,
         gamma: int = 1,
         groups: int = 1,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
     ) -> None:
         super().__init__()
 
         self.in_channels = in_channels
+        self.alpha = alpha
+        self.gamma = gamma
+        self.groups = groups
         self.num_estimators = num_estimators
         self.in_planes = 64
         block_planes = self.in_planes
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.conv1 = PackedConv2d(
                 self.in_channels,
                 block_planes,
                 kernel_size=7,
                 stride=2,
                 padding=3,
                 alpha=alpha,
@@ -242,15 +238,15 @@
                 groups=groups,
                 bias=False,
                 first=True,
             )
 
         self.bn1 = nn.BatchNorm2d(block_planes * alpha)
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
             self.optional_pool = nn.Identity()
 
         self.layer1 = self._make_layer(
@@ -346,23 +342,32 @@
         )
 
         out = self.pool(out)
         out = self.flatten(out)
         out = self.linear(out)
         return out
 
+    def check_config(self, config: Dict[str, Any]) -> bool:
+        """Check if the pretrained configuration matches the current model."""
+        return (
+            (config["alpha"] == self.alpha)
+            * (config["gamma"] == self.gamma)
+            * (config["groups"] == self.groups)
+            * (config["num_estimators"] == self.num_estimators)
+        )
+
 
 def packed_resnet18(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
     groups: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
     pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-18 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
@@ -379,32 +384,37 @@
         num_blocks=[2, 2, 2, 2],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
-    if pretrained:
-        weights = weight_ids[str(num_classes)][18]
+    if pretrained:  # coverage: ignore
+        weights = weight_ids[str(num_classes)]["18"]
         if weights is None:
             raise ValueError("No pretrained weights for this configuration")
-        net.load_state_dict(load_hf(weights))
+        state_dict, config = load_hf(weights)
+        if not net.check_config(config):
+            raise ValueError(
+                "Pretrained weights do not match current configuration."
+            )
+        net.load_state_dict(state_dict)
     return net
 
 
 def packed_resnet34(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
     groups: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
     pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-34 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
@@ -421,32 +431,37 @@
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
-    if pretrained:
-        weights = weight_ids[str(num_classes)][34]
+    if pretrained:  # coverage: ignore
+        weights = weight_ids[str(num_classes)]["34"]
         if weights is None:
             raise ValueError("No pretrained weights for this configuration")
-        net.load_state_dict(load_hf(weights))
+        state_dict, config = load_hf(weights)
+        if not net.check_config(config):
+            raise ValueError(
+                "Pretrained weights do not match current configuration."
+            )
+        net.load_state_dict(state_dict)
     return net
 
 
 def packed_resnet50(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
     groups: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
     pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-50 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
@@ -463,32 +478,37 @@
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
-    if pretrained:
-        weights = weight_ids[str(num_classes)][50]
+    if pretrained:  # coverage: ignore
+        weights = weight_ids[str(num_classes)]["50"]
         if weights is None:
             raise ValueError("No pretrained weights for this configuration")
-        net.load_state_dict(load_hf(weights))
+        state_dict, config = load_hf(weights)
+        if not net.check_config(config):
+            raise ValueError(
+                "Pretrained weights do not match current configuration."
+            )
+        net.load_state_dict(state_dict)
     return net
 
 
 def packed_resnet101(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
     groups: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
     pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-101 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
@@ -505,59 +525,69 @@
         num_blocks=[3, 4, 23, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
-    if pretrained:
-        weights = weight_ids[str(num_classes)][101]
+    if pretrained:  # coverage: ignore
+        weights = weight_ids[str(num_classes)]["101"]
         if weights is None:
             raise ValueError("No pretrained weights for this configuration")
-        net.load_state_dict(load_hf(weights))
+        state_dict, config = load_hf(weights)
+        if not net.check_config(config):
+            raise ValueError(
+                "Pretrained weights do not match current configuration."
+            )
+        net.load_state_dict(state_dict)
     return net
 
 
 def packed_resnet152(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     num_classes: int,
     groups: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
     pretrained: bool = False,
 ) -> _PackedResNet:
     """Packed-Ensembles of ResNet-152 from `Deep Residual Learning for Image
     Recognition <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         alpha (int): Expansion factor affecting the width of the estimators.
         gamma (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _PackedResNet: A Packed-Ensembles ResNet-152.
     """
     net = _PackedResNet(
         block=Bottleneck,
         num_blocks=[3, 8, 36, 3],
         in_channels=in_channels,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
-    if pretrained:
-        weights = weight_ids[str(num_classes)][152]
+    if pretrained:  # coverage: ignore
+        weights = weight_ids[str(num_classes)]["152"]
         if weights is None:
             raise ValueError("No pretrained weights for this configuration")
-        net.load_state_dict(load_hf(weights))
+        state_dict, config = load_hf(weights)
+        if not net.check_config(config):
+            raise ValueError(
+                "Pretrained weights do not match current configuration."
+            )
+        net.load_state_dict(state_dict)
     return net
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/models/resnet/std.py` & `torch_uncertainty-0.1.3/torch_uncertainty/models/resnet/std.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,17 @@
         out = F.relu(out)
         return out
 
 
 class Bottleneck(nn.Module):
     expansion = 4
 
-    def __init__(self, in_planes, planes, stride=1, groups=1):
+    def __init__(
+        self, in_planes: int, planes: int, stride: int = 1, groups: int = 1
+    ):
         super(Bottleneck, self).__init__()
 
         self.conv1 = nn.Conv2d(
             in_planes,
             planes,
             kernel_size=1,
             groups=groups,
@@ -130,22 +132,22 @@
     def __init__(
         self,
         block: Type[Union[BasicBlock, Bottleneck]],
         num_blocks: List[int],
         in_channels: int,
         num_classes: int,
         groups: int,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
     ) -> None:
         super().__init__()
 
         self.in_planes = 64
         block_planes = self.in_planes
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.conv1 = nn.Conv2d(
                 in_channels,
                 block_planes,
                 kernel_size=7,
                 stride=2,
                 padding=3,
                 groups=1,  # No groups in the first layer
@@ -160,15 +162,15 @@
                 padding=1,
                 groups=1,  # No groups in the first layer
                 bias=False,
             )
 
         self.bn1 = nn.BatchNorm2d(block_planes)
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
             self.optional_pool = nn.Identity()
 
         self.layer1 = self._make_layer(
@@ -243,147 +245,147 @@
         return out
 
 
 def resnet18(
     in_channels: int,
     num_classes: int,
     groups: int = 1,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _ResNet:
     """ResNet-18 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
         groups (int): Number of groups in convolutions. Defaults to 1.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _ResNet: A ResNet-18.
     """
     return _ResNet(
         block=BasicBlock,
         num_blocks=[2, 2, 2, 2],
         in_channels=in_channels,
         num_classes=num_classes,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def resnet34(
     in_channels: int,
     num_classes: int,
     groups: int = 1,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _ResNet:
     """ResNet-34 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
         groups (int): Number of groups in convolutions. Defaults to 1.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _ResNet: A ResNet-34.
     """
     return _ResNet(
         block=BasicBlock,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def resnet50(
     in_channels: int,
     num_classes: int,
     groups: int = 1,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _ResNet:
     """ResNet-50 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
         groups (int): Number of groups in convolutions. Defaults to 1.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _ResNet: A ResNet-50.
     """
     return _ResNet(
         block=Bottleneck,
         num_blocks=[3, 4, 6, 3],
         in_channels=in_channels,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def resnet101(
     in_channels: int,
     num_classes: int,
     groups: int = 1,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _ResNet:
     """ResNet-101 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
         groups (int): Number of groups in convolutions. Defaults to 1.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _ResNet: A ResNet-101.
     """
     return _ResNet(
         block=Bottleneck,
         num_blocks=[3, 4, 23, 3],
         in_channels=in_channels,
         groups=groups,
         num_classes=num_classes,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
 
 
 def resnet152(
     in_channels: int,
     num_classes: int,
     groups: int = 1,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _ResNet:
     """ResNet-152 from `Deep Residual Learning for Image Recognition
     <https://arxiv.org/pdf/1512.03385.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_classes (int): Number of classes to predict.
         groups (int, optional): Number of groups in convolutions. Defaults to
             ``1``.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _ResNet: A ResNet-152.
     """
     return _ResNet(
         block=Bottleneck,
         num_blocks=[3, 8, 36, 3],
         in_channels=in_channels,
         num_classes=num_classes,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/batched.py` & `torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/batched.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,27 +70,27 @@
         depth: int,
         widen_factor: int,
         in_channels: int,
         num_classes: int,
         num_estimators: int,
         groups: int = 1,
         dropout_rate: float = 0.0,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
     ) -> None:
         super().__init__()
         self.num_estimators = num_estimators
         self.in_planes = 16
 
         assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4."
         n = (depth - 4) / 6
         k = widen_factor
 
         nStages = [16, 16 * k, 32 * k, 64 * k]
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.conv1 = BatchConv2d(
                 in_channels,
                 nStages[0],
                 num_estimators=self.num_estimators,
                 groups=groups,
                 kernel_size=7,
                 stride=2,
@@ -105,15 +105,15 @@
                 groups=groups,
                 kernel_size=3,
                 stride=1,
                 padding=1,
                 bias=True,
             )
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
             self.optional_pool = nn.Identity()
 
         self.layer1 = self._wide_layer(
@@ -199,32 +199,32 @@
 
 
 def batched_wideresnet28x10(
     in_channels: int,
     num_estimators: int,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _BatchedWide:
     """BatchEnsemble of Wide-ResNet-28x10 from `Wide Residual Networks
     <https://arxiv.org/pdf/1605.07146.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         num_classes (int): Number of classes to predict.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _BatchedWide: A BatchEnsemble-style Wide-ResNet-28x10.
     """
     return _BatchedWide(
         in_channels=in_channels,
         depth=28,
         widen_factor=10,
         dropout_rate=0.3,
         num_classes=num_classes,
         num_estimators=num_estimators,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/masked.py` & `torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/masked.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,27 +75,27 @@
         widen_factor: int,
         in_channels: int,
         num_classes: int,
         num_estimators: int,
         scale: float = 2.0,
         groups: int = 1,
         dropout_rate: float = 0.0,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
     ):
         super().__init__()
         self.num_estimators = num_estimators
         self.in_planes = 16
 
         assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4."
         n = (depth - 4) / 6
         k = widen_factor
 
         nStages = [16, 16 * k, 32 * k, 64 * k]
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.conv1 = nn.Conv2d(
                 in_channels,
                 nStages[0],
                 kernel_size=7,
                 stride=2,
                 padding=3,
                 bias=True,
@@ -108,15 +108,15 @@
                 kernel_size=3,
                 stride=1,
                 padding=1,
                 bias=True,
                 groups=1,
             )
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
             self.optional_pool = nn.Identity()
 
         self.layer1 = self._wide_layer(
@@ -206,35 +206,35 @@
 
 def masked_wideresnet28x10(
     in_channels: int,
     num_estimators: int,
     scale: float,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _MaskedWide:
     """Masksembles of Wide-ResNet-28x10 from `Wide Residual Networks
     <https://arxiv.org/pdf/1605.07146.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         scale (float): Expansion factor affecting the width of the estimators.
         groups (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _MaskedWide: A Masksembles-style Wide-ResNet-28x10.
     """
     return _MaskedWide(
         in_channels=in_channels,
         depth=28,
         widen_factor=10,
         dropout_rate=0.3,
         num_classes=num_classes,
         num_estimators=num_estimators,
         scale=scale,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/packed.py` & `torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/packed.py`

 * *Files 15% similar despite different names*

```diff
@@ -83,27 +83,27 @@
         in_channels: int,
         num_classes: int,
         num_estimators: int = 4,
         alpha: int = 2,
         gamma: int = 1,
         groups: int = 1,
         dropout_rate: float = 0,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
     ):
         super().__init__()
         self.num_estimators = num_estimators
         self.in_planes = 16
 
         assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4."
         num_blocks = int((depth - 4) / 6)
         k = widen_factor
 
         nStages = [16, 16 * k, 32 * k, 64 * k]
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.conv1 = PackedConv2d(
                 in_channels,
                 nStages[0],
                 kernel_size=7,
                 alpha=alpha,
                 num_estimators=self.num_estimators,
                 stride=2,
@@ -124,15 +124,15 @@
                 padding=1,
                 gamma=gamma,
                 groups=groups,
                 bias=True,
                 first=True,
             )
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
             self.optional_pool = nn.Identity()
 
         self.layer1 = self._wide_layer(
@@ -233,26 +233,26 @@
 def packed_wideresnet28x10(
     in_channels: int,
     num_estimators: int,
     alpha: int,
     gamma: int,
     groups: int,
     num_classes: int,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> _PackedWide:
     """Packed-Ensembles of Wide-ResNet-28x10 from `Wide Residual Networks
     <https://arxiv.org/pdf/1605.07146.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels.
         num_estimators (int): Number of estimators in the ensemble.
         alpha (int): Expansion factor affecting the width of the estimators.
         gamma (int): Number of groups within each estimator.
         num_classes (int): Number of classes to predict.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _PackedWide: A Packed-Ensembles Wide-ResNet-28x10.
     """
     return _PackedWide(
         in_channels=in_channels,
@@ -260,9 +260,9 @@
         widen_factor=10,
         num_classes=num_classes,
         dropout_rate=0.3,
         num_estimators=num_estimators,
         alpha=alpha,
         gamma=gamma,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/models/wideresnet/std.py` & `torch_uncertainty-0.1.3/torch_uncertainty/models/wideresnet/std.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,26 +65,26 @@
         self,
         depth: int,
         widen_factor: int,
         in_channels: int,
         num_classes: int,
         dropout_rate: float,
         groups: int = 1,
-        imagenet_structure: bool = True,
+        style: str = "imagenet",
     ):
         super().__init__()
         self.in_planes = 16
 
         assert (depth - 4) % 6 == 0, "Wide-resnet depth should be 6n+4."
         num_blocks = int((depth - 4) / 6)
         k = widen_factor
 
         nStages = [16, 16 * k, 32 * k, 64 * k]
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.conv1 = nn.Conv2d(
                 in_channels,
                 nStages[0],
                 kernel_size=7,
                 stride=2,
                 padding=3,
                 groups=groups,
@@ -97,15 +97,15 @@
                 kernel_size=3,
                 stride=1,
                 padding=1,
                 groups=groups,
                 bias=True,
             )
 
-        if imagenet_structure:
+        if style == "imagenet":
             self.optional_pool = nn.MaxPool2d(
                 kernel_size=3, stride=2, padding=1
             )
         else:
             self.optional_pool = nn.Identity()
 
         self.layer1 = self._wide_layer(
@@ -182,32 +182,32 @@
         return out
 
 
 def wideresnet28x10(
     in_channels: int,
     num_classes: int,
     groups: int = 1,
-    imagenet_structure: bool = True,
+    style: str = "imagenet",
 ) -> nn.Module:
     """Wide-ResNet-28x10 from `Wide Residual Networks
     <https://arxiv.org/pdf/1605.07146.pdf>`_.
 
     Args:
         in_channels (int): Number of input channels
         num_classes (int): Number of classes to predict.
         groups (int, optional): Number of groups in convolutions. Defaults to
             ``1``.
-        imagenet_structure (bool, optional): Whether to use the ImageNet
+        style (bool, optional): Whether to use the ImageNet
             structure. Defaults to ``True``.
 
     Returns:
         _Wide: A Wide-ResNet-28x10.
     """
     return _Wide(
         depth=28,
         widen_factor=10,
         in_channels=in_channels,
         dropout_rate=0.3,
         num_classes=num_classes,
         groups=groups,
-        imagenet_structure=imagenet_structure,
+        style=style,
     )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/optimization_procedures.py` & `torch_uncertainty-0.1.3/torch_uncertainty/optimization_procedures.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 from timm.optim import Lamb
 
 # fmt:on
 __all__ = [
     "optim_cifar10_resnet18",
     "optim_cifar10_resnet50",
     "optim_cifar10_wideresnet",
+    "optim_cifar10_vgg16",
     "optim_cifar100_resnet18",
     "optim_cifar100_resnet50",
+    "optim_cifar100_vgg16",
     "optim_imagenet_resnet50",
     "optim_imagenet_resnet50_A3",
+    "optim_regression",
 ]
 
 
 def optim_cifar10_resnet18(model: nn.Module) -> dict:
     """optimizer to train a ResNet18 on CIFAR-10"""
     optimizer = optim.SGD(
         model.parameters(),
@@ -66,26 +69,41 @@
         optimizer,
         milestones=[60, 120, 160],
         gamma=0.2,
     )
     return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
 
+def optim_cifar10_vgg16(model: nn.Module) -> dict:
+    """optimizer to train a VGG16 on CIFAR-10"""
+    optimizer = optim.Adam(
+        model.parameters(),
+        lr=0.005,
+        weight_decay=1e-6,
+    )
+    scheduler = optim.lr_scheduler.MultiStepLR(
+        optimizer,
+        milestones=[25, 50],
+        gamma=0.1,
+    )
+    return {"optimizer": optimizer, "lr_scheduler": scheduler}
+
+
 def optim_cifar100_resnet18(model: nn.Module) -> dict:
     optimizer = optim.SGD(
         model.parameters(),
         lr=0.1,
         momentum=0.9,
-        weight_decay=1e-4,
+        weight_decay=5e-4,
         nesterov=True,
     )
     scheduler = optim.lr_scheduler.MultiStepLR(
         optimizer,
-        milestones=[60, 120, 160],
-        gamma=0.2,
+        milestones=[25, 50],
+        gamma=0.1,
     )
     return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
 
 def optim_cifar100_resnet50(model: nn.Module) -> dict:
     r"""Hyperparameters from Deep Residual Learning for Image Recognition
     https://arxiv.org/pdf/1512.03385.pdf
@@ -101,14 +119,31 @@
         optimizer,
         milestones=[60, 120, 160],
         gamma=0.2,
     )
     return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
 
+def optim_cifar100_vgg16(model: nn.Module) -> dict:
+    """optimizer to train a VGG16 on CIFAR-100"""
+    optimizer = optim.SGD(
+        model.parameters(),
+        lr=0.05,
+        momentum=0.9,
+        weight_decay=1e-4,
+        nesterov=True,
+    )
+    scheduler = optim.lr_scheduler.MultiStepLR(
+        optimizer,
+        milestones=[60, 120, 160],
+        gamma=0.2,
+    )
+    return {"optimizer": optimizer, "lr_scheduler": scheduler}
+
+
 def optim_imagenet_resnet50(
     model: nn.Module,
     num_epochs: int = 90,
     start_lr: float = 0.256,
     end_lr: float = 0,
 ) -> dict:
     r"""Hyperparameters from Deep Residual Learning for Image Recognition
@@ -175,14 +210,29 @@
             "interval": "step",
             "frequency": 1,
         },
         "monitor": "hp/val_acc",
     }
 
 
+def optim_regression(
+    model: nn.Module,
+    learning_rate: float = 1e-2,
+) -> dict:
+    optimizer = optim.SGD(
+        model.parameters(),
+        lr=learning_rate,
+        weight_decay=0,
+    )
+    return {
+        "optimizer": optimizer,
+        "monitor": "hp/val_nll",
+    }
+
+
 def batch_ensemble_wrapper(model: nn.Module, optimization_procedure: Callable):
     procedure = optimization_procedure(model)
     param_optimizer = procedure["optimizer"]
     scheduler = procedure["lr_scheduler"]
 
     weight_decay = param_optimizer.defaults["weight_decay"]
     lr = param_optimizer.defaults["lr"]
@@ -215,15 +265,18 @@
     )
 
     scheduler.optimizer = optimizer
     return {"optimizer": optimizer, "lr_scheduler": scheduler}
 
 
 def get_procedure(
-    arch_name: str, ds_name: str, model_name: str = ""
+    arch_name: str,
+    ds_name: str,
+    model_name: str = "",
+    imagenet_recipe: str = None,
 ) -> Callable:
     """Get the optimization procedure for a given architecture and dataset.
 
     Args:
         arch_name (str): The name of the architecture.
         ds_name (str): The name of the dataset.
         model_name (str, optional): The name of the model. Defaults to "".
@@ -239,21 +292,33 @@
         else:
             raise NotImplementedError(f"Dataset {ds_name} not implemented.")
     elif arch_name == "resnet50":
         if ds_name == "cifar10":
             procedure = optim_cifar10_resnet50
         elif ds_name == "cifar100":
             procedure = optim_cifar100_resnet50
+        elif ds_name == "imagenet":
+            if imagenet_recipe is not None and imagenet_recipe == "A3":
+                procedure = optim_imagenet_resnet50_A3
+            else:
+                procedure = optim_imagenet_resnet50
         else:
             raise NotImplementedError(f"Dataset {ds_name} not implemented.")
     elif arch_name == "wideresnet28x10":
         if ds_name == "cifar10" or ds_name == "cifar100":
             procedure = optim_cifar10_wideresnet
         else:
             raise NotImplementedError(f"Dataset {ds_name} not implemented.")
+    elif arch_name == "vgg16":
+        if ds_name == "cifar10":
+            procedure = optim_cifar10_vgg16
+        elif ds_name == "cifar100":
+            procedure = optim_cifar100_vgg16
+        else:
+            raise NotImplementedError(f"Dataset {ds_name} not implemented.")
     else:
         raise NotImplementedError(f"Architecture {arch_name} not implemented.")
 
     if model_name == "batched":
         procedure = partial(
             batch_ensemble_wrapper, optimization_procedure=procedure
         )
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/post_processing/temperature_scaler.py` & `torch_uncertainty-0.1.3/torch_uncertainty/post_processing/temperature_scaler.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 # fmt: off
+from typing import Literal, Optional
+
 import torch
 from torch import nn, optim
 from torch.utils.data import DataLoader
+from tqdm import tqdm
 
 
 # fmt: on
 class TemperatureScaler(nn.Module):
     """
     Temperature scaling post-processing for calibrated probabilities.
 
     Args:
         init_value (float, optional): Initial value for the temperature.
             Defaults to 1.
+        lr (float, optional): Learning rate for the optimizer. Defaults to 0.1.
+        max_iter (int, optional): Maximum number of iterations for the
+            optimizer. Defaults to 100.
+        device (Optional[Literal["cpu", "cuda"]], optional): Device to use
+            for optimization. Defaults to None.
 
     Reference:
         Guo, C., Pleiss, G., Sun, Y., & Weinberger, K. Q. On calibration
             of modern neural networks. In ICML 2017.
 
     Note:
         Inspired by `<https://github.com/gpleiss/temperature_scaling>`_
     """
 
     trained = False
 
     def __init__(
         self,
         init_val: float = 1,
-        lr: float = 0.01,
-        max_iter: int = 50,
-        device=None,
+        lr: float = 0.1,
+        max_iter: int = 100,
+        device: Optional[Literal["cpu", "cuda"]] = None,
     ) -> None:
         super().__init__()
         self.device = device
         if init_val <= 0:
             raise ValueError("Initial temperature value must be positive.")
 
-        self.temperature = nn.Parameter(torch.ones(1) * init_val).to(device)
+        self.temperature = nn.Parameter(
+            torch.ones(1, device=device) * init_val, requires_grad=True
+        )
         self.criterion = nn.CrossEntropyLoss()
 
         if lr <= 0:
             raise ValueError("Learning rate must be positive.")
         self.lr = lr
 
         if max_iter <= 0:
@@ -52,70 +62,90 @@
 
         Args:
             val (float): Temperature value.
         """
         if val <= 0:
             raise ValueError("Temperature value must be positive.")
 
-        self.temperature = nn.Parameter(torch.ones(1) * val)
+        self.temperature = nn.Parameter(
+            torch.ones(1, device=self.device) * val, requires_grad=True
+        )
 
     def fit(
-        self, model: nn.Module, val_loader: DataLoader
+        self,
+        model: nn.Module,
+        calib_loader: DataLoader,
+        save_logits: bool = False,
+        progress: bool = True,
     ) -> "TemperatureScaler":
         """
         Fit the temperature to the validation data.
 
         Args:
             model (nn.Module): Model to calibrate.
-            val_loader (DataLoader): Validation dataloader.
+            calib_loader (DataLoader): Calibration dataloader.
+            save_logits (bool, optional): Whether to save the logits and
+                labels. Defaults to False.
+            progress (bool, optional): Whether to show a progress bar.
+                Defaults to True.
 
         Returns:
             TemperatureScaler: Calibrated scaler.
         """
         logits_list = []
         labels_list = []
         with torch.no_grad():
-            for input, label in val_loader:
+            for input, label in tqdm(calib_loader, disable=not progress):
                 input = input.to(self.device)
                 logits = model(input)
                 logits_list.append(logits)
                 labels_list.append(label)
-            logits = torch.cat(logits_list).to(self.device)
-            labels = torch.cat(labels_list).to(self.device)
+        logits = torch.cat(logits_list).detach().to(self.device)
+        labels = torch.cat(labels_list).detach().to(self.device)
 
         optimizer = optim.LBFGS(
             [self.temperature], lr=self.lr, max_iter=self.max_iter
         )
 
-        def eval() -> torch.Tensor:
+        def eval() -> float:
             optimizer.zero_grad()
             loss = self.criterion(self._scale(logits), labels)
             loss.backward()
             return loss
 
         optimizer.step(eval)
         self.trained = True
-
+        if save_logits:
+            self.logits = logits
+            self.labels = labels
         return self
 
     def forward(self, logits: torch.Tensor) -> torch.Tensor:
-        if not self.trained:
-            print(
-                "TemperatureScaler has not been trained yet. Returning a "
-                "manually tempered input."
-            )
-        return self._scale(logits)
+        with torch.no_grad():
+            if not self.trained:
+                print(
+                    "TemperatureScaler has not been trained yet. Returning a "
+                    "manually tempered input."
+                )
+            return self._scale(logits)
 
     def _scale(self, logits: torch.Tensor) -> torch.Tensor:
         """
-        Scale the logits by the temperature.
+        Scale the logits with the optimal temperature.
 
         Args:
-            logits (torch.Tensor): Logits to scale.
+            logits (torch.Tensor): Logits to be scaled.
 
         Returns:
             torch.Tensor: Scaled logits.
         """
         temperature = self.temperature.unsqueeze(1).expand(
             logits.size(0), logits.size(1)
         )
         return logits / temperature
+
+    def fit_predict(
+        self, model: nn.Module, calib_loader: DataLoader, progress: bool = True
+    ) -> torch.Tensor:
+        self.fit(model, calib_loader, save_logits=True, progress=progress)
+        calib_logits = self(self.logits)
+        return calib_logits
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/routines/classification.py` & `torch_uncertainty-0.1.3/torch_uncertainty/routines/classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # fmt: off
 from argparse import ArgumentParser, Namespace
-from typing import Any, List, Tuple, Union
+from typing import Any, List, Optional, Tuple, Type, Union
 
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from einops import rearrange
 from pytorch_lightning.utilities.memory import get_model_size_mb
@@ -15,94 +15,122 @@
     AveragePrecision,
     CalibrationError,
     MetricCollection,
 )
 
 from ..metrics import (
     FPR95,
+    BrierScore,
     Disagreement,
     Entropy,
     MutualInformation,
     NegativeLogLikelihood,
     VariationRatio,
 )
 
 
 # fmt:on
 class ClassificationSingle(pl.LightningModule):
     """
     Args:
+        ood_detection (bool, optional): Indicates whether to evaluate the OOD
+            detection performance or not. Defaults to ``False``.
         use_entropy (bool, optional): Indicates whether to use the entropy
             values as the OOD criterion or not. Defaults to ``False``.
         use_logits (bool, optional): Indicates whether to use the logits as the
             OOD criterion or not. Defaults to ``False``.
 
     Note:
-        The default OOD criterion is the confidence score.
+        The default OOD criterion is the softmax confidence score.
 
     Warning:
         Make sure at most only one of :attr:`use_entropy` and :attr:`use_logits`
         attributes is set to ``True``. Otherwise a :class:`ValueError()` will
         be raised.
     """
 
     def __init__(
         self,
         num_classes: int,
         model: nn.Module,
-        loss: nn.Module,
+        loss: Type[nn.Module],
         optimization_procedure: Any,
+        ood_detection: bool = False,
         use_entropy: bool = False,
         use_logits: bool = False,
         **kwargs,
     ) -> None:
         super().__init__()
 
+        self.save_hyperparameters(
+            ignore=[
+                "model",
+                "loss",
+                "optimization_procedure",
+            ]
+        )
+
         if (use_logits + use_entropy) > 1:
             raise ValueError("You cannot choose more than one OOD criterion.")
 
         self.num_classes = num_classes
+        self.ood_detection = ood_detection
         self.use_logits = use_logits
         self.use_entropy = use_entropy
 
+        self.binary_cls = num_classes == 1
+
         # model
         self.model = model
         # loss
         self.loss = loss
         # optimization procedure
         self.optimization_procedure = optimization_procedure
-        # metrics
-        cls_metrics = MetricCollection(
-            {
-                "nll": NegativeLogLikelihood(),
-                "acc": Accuracy(
-                    task="multiclass", num_classes=self.num_classes
-                ),
-                "ece": CalibrationError(
-                    task="multiclass", num_classes=self.num_classes
-                ),
-            },
-            compute_groups=False,
-        )
 
-        ood_metrics = MetricCollection(
-            {
-                "fpr95": FPR95(pos_label=1),
-                "auroc": AUROC(task="binary"),
-                "aupr": AveragePrecision(task="binary"),
-            },
-            compute_groups=[["auroc", "aupr"], ["fpr95"]],
-        )
+        # metrics
+        if self.binary_cls:
+            cls_metrics = MetricCollection(
+                {
+                    "acc": Accuracy(task="binary"),
+                    "ece": CalibrationError(task="binary"),
+                    "brier": BrierScore(num_classes=1),
+                },
+                compute_groups=False,
+            )
+        else:
+            cls_metrics = MetricCollection(
+                {
+                    "nll": NegativeLogLikelihood(),
+                    "acc": Accuracy(
+                        task="multiclass", num_classes=self.num_classes
+                    ),
+                    "ece": CalibrationError(
+                        task="multiclass", num_classes=self.num_classes
+                    ),
+                    "brier": BrierScore(num_classes=self.num_classes),
+                },
+                compute_groups=False,
+            )
 
-        self.val_metrics = cls_metrics.clone(prefix="hp/val_")
+        self.val_cls_metrics = cls_metrics.clone(prefix="hp/val_")
         self.test_cls_metrics = cls_metrics.clone(prefix="hp/test_")
-        self.test_ood_metrics = ood_metrics.clone(prefix="hp/test_")
 
         self.test_entropy_id = Entropy()
-        self.test_entropy_ood = Entropy()
+
+        if self.ood_detection:
+            ood_metrics = MetricCollection(
+                {
+                    "fpr95": FPR95(pos_label=1),
+                    "auroc": AUROC(task="binary"),
+                    "aupr": AveragePrecision(task="binary"),
+                },
+                compute_groups=[["auroc", "aupr"], ["fpr95"]],
+            )
+            self.test_ood_metrics = ood_metrics.clone(prefix="hp/test_")
+            self.test_entropy_ood = Entropy()
 
     def configure_optimizers(self) -> Any:
         return self.optimization_procedure(self)
 
     @property
     def criterion(self) -> nn.Module:
         return self.loss()
@@ -119,74 +147,91 @@
                 Namespace(**param),
                 {
                     "hp/val_nll": 0,
                     "hp/val_acc": 0,
                     "hp/test_acc": 0,
                     "hp/test_nll": 0,
                     "hp/test_ece": 0,
+                    "hp/test_brier": 0,
                     "hp/test_entropy_id": 0,
                     "hp/test_entropy_ood": 0,
                     "hp/test_aupr": 0,
                     "hp/test_auroc": 0,
                     "hp/test_fpr95": 0,
                 },
             )
 
     def training_step(
         self, batch: Tuple[torch.Tensor, torch.Tensor], batch_idx: int
     ) -> STEP_OUTPUT:
         inputs, targets = batch
         logits = self.forward(inputs)
+
+        # BCEWithLogitsLoss expects float targets
+        if self.loss == nn.BCEWithLogitsLoss:
+            targets = targets.float()
         loss = self.criterion(logits, targets)
         self.log("train_loss", loss)
         return loss
 
     def validation_step(
         self, batch: Tuple[torch.Tensor, torch.Tensor], batch_idx: int
     ) -> None:
         inputs, targets = batch
         logits = self.forward(inputs)
-        probs = F.softmax(logits, dim=-1)
-        self.val_metrics.update(probs, targets)
+
+        if self.binary_cls:
+            probs = torch.sigmoid(logits).squeeze(-1)
+        else:
+            probs = F.softmax(logits, dim=-1)
+
+        self.val_cls_metrics.update(probs, targets)
 
     def validation_epoch_end(
         self, outputs: Union[EPOCH_OUTPUT, List[EPOCH_OUTPUT]]
     ) -> None:
-        self.log_dict(self.val_metrics.compute())
-        self.val_metrics.reset()
+        self.log_dict(self.val_cls_metrics.compute())
+        self.val_cls_metrics.reset()
 
     def test_step(
         self,
         batch: Tuple[torch.Tensor, torch.Tensor],
         batch_idx: int,
-        dataloader_idx: int,
+        dataloader_idx: Optional[int] = 0,
     ) -> None:
         inputs, targets = batch
         logits = self.forward(inputs)
-        probs = F.softmax(logits, dim=-1)
+
+        if self.binary_cls:
+            probs = torch.sigmoid(logits).squeeze(-1)
+        else:
+            probs = F.softmax(logits, dim=-1)
         confs, _ = probs.max(dim=-1)
 
         if self.use_logits:
             ood_values, _ = -logits.max(dim=-1)
         elif self.use_entropy:
             ood_values = torch.special.entr(probs).sum(dim=-1)
         else:
             ood_values = -confs
 
         if dataloader_idx == 0:
-            self.test_cls_metrics.update(probs, targets, num_classes=10)
-            self.test_ood_metrics.update(ood_values, torch.zeros_like(targets))
+            self.test_cls_metrics.update(probs, targets)
             self.test_entropy_id(probs)
             self.log(
                 "hp/test_entropy_id",
                 self.test_entropy_id,
                 on_epoch=True,
                 add_dataloader_idx=False,
             )
-        else:
+            if self.ood_detection:
+                self.test_ood_metrics.update(
+                    ood_values, torch.zeros_like(targets)
+                )
+        elif self.ood_detection and dataloader_idx == 1:
             self.test_ood_metrics.update(ood_values, torch.ones_like(targets))
             self.test_entropy_ood(probs)
             self.log(
                 "hp/test_entropy_ood",
                 self.test_entropy_ood,
                 on_epoch=True,
                 add_dataloader_idx=False,
@@ -194,26 +239,29 @@
 
     def test_epoch_end(
         self, outputs: Union[EPOCH_OUTPUT, List[EPOCH_OUTPUT]]
     ) -> None:
         self.log_dict(
             self.test_cls_metrics.compute(),
         )
-        self.log_dict(
-            self.test_ood_metrics.compute(),
-        )
         self.test_cls_metrics.reset()
-        self.test_ood_metrics.reset()
+
+        if self.ood_detection:
+            self.log_dict(
+                self.test_ood_metrics.compute(),
+            )
+            self.test_ood_metrics.reset()
 
     @staticmethod
     def add_model_specific_args(
         parent_parser: ArgumentParser,
     ) -> ArgumentParser:
         """Defines the routine's attributes via command-line options:
 
+        - ``--evaluate_ood``: sets :attr:`ood_detection` to ``True``.
         - ``--entropy``: sets :attr:`use_entropy` to ``True``.
         - ``--logits``: sets :attr:`use_logits` to ``True``.
         """
         parent_parser.add_argument(
             "--entropy", dest="use_entropy", action="store_true"
         )
         parent_parser.add_argument(
@@ -221,50 +269,54 @@
         )
         return parent_parser
 
 
 class ClassificationEnsemble(ClassificationSingle):
     """
     Args:
+        ood_detection (bool, optional): Indicates whether to evaluate the OOD
+            detection performance or not. Defaults to ``False``.
         use_entropy (bool, optional): Indicates whether to use the entropy
             values as the OOD criterion or not. Defaults to ``False``.
         use_logits (bool, optional): Indicates whether to use the logits as the
             OOD criterion or not. Defaults to ``False``.
         use_mi (bool, optional): Indicates whether to use the mutual
             information as the OOD criterion or not. Defaults to ``False``.
         use_variation_ratio (bool, optional): Indicates whether to use the
             variation ratio as the OOD criterion or not. Defaults to ``False``.
 
     Note:
-        The default OOD criterion is the confidence score.
+        The default OOD criterion is the averaged softmax confidence score.
 
     Warning:
         Make sure at most only one of :attr:`use_entropy`, :attr:`use_logits`
         , :attr:`use_mi`, and :attr:`use_variation_ratio` attributes is set to
         ``True``. Otherwise a :class:`ValueError()` will be raised.
     """
 
     def __init__(
         self,
         num_classes: int,
         model: nn.Module,
-        loss: nn.Module,
+        loss: Type[nn.Module],
         optimization_procedure: Any,
         num_estimators: int,
+        ood_detection: bool = False,
         use_entropy: bool = False,
         use_logits: bool = False,
         use_mi: bool = False,
         use_variation_ratio: bool = False,
         **kwargs,
     ) -> None:
         super().__init__(
             num_classes=num_classes,
             model=model,
             loss=loss,
             optimization_procedure=optimization_procedure,
+            ood_detection=ood_detection,
             use_entropy=use_entropy,
             use_logits=use_logits,
             **kwargs,
         )
 
         self.num_estimators = num_estimators
 
@@ -284,29 +336,34 @@
             {
                 "disagreement": Disagreement(),
                 "mi": MutualInformation(),
                 "entropy": Entropy(),
             }
         )
         self.test_id_ens_metrics = ens_metrics.clone(prefix="hp/test_id_ens_")
-        self.test_ood_ens_metrics = ens_metrics.clone(prefix="hp/test_ood_ens_")
+
+        if self.ood_detection:
+            self.test_ood_ens_metrics = ens_metrics.clone(
+                prefix="hp/test_ood_ens_"
+            )
 
     def on_train_start(self) -> None:
         # hyperparameters for performances
         param = {}
         param["storage"] = f"{get_model_size_mb(self)} MB"
         if self.logger is not None:
             self.logger.log_hyperparams(
                 Namespace(**param),
                 {
                     "hp/val_nll": 0,
                     "hp/val_acc": 0,
                     "hp/test_acc": 0,
                     "hp/test_nll": 0,
                     "hp/test_ece": 0,
+                    "hp/test_brier": 0,
                     "hp/test_entropy_id": 0,
                     "hp/test_entropy_ood": 0,
                     "hp/test_aupr": 0,
                     "hp/test_auroc": 0,
                     "hp/test_fpr95": 0,
                     "hp/test_id_ens_disagreement": 0,
                     "hp/test_id_ens_mi": 0,
@@ -317,37 +374,48 @@
                 },
             )
 
     def training_step(
         self, batch: Tuple[torch.Tensor, torch.Tensor], batch_idx: int
     ) -> STEP_OUTPUT:
         inputs, targets = batch
+
+        # eventual input repeat is done in the model
         targets = targets.repeat(self.num_estimators)
         return super().training_step((inputs, targets), batch_idx)
 
     def validation_step(  # type: ignore
         self, batch: Tuple[torch.Tensor, torch.Tensor], batch_idx: int
     ) -> None:
         inputs, targets = batch
         logits = self.forward(inputs)
-        logits = rearrange(logits, "(n b) c -> b n c", n=self.num_estimators)
-        probs_per_est = F.softmax(logits, dim=-1)
+        logits = rearrange(logits, "(m b) c -> b m c", m=self.num_estimators)
+        if self.binary_cls:
+            probs_per_est = torch.sigmoid(logits).squeeze(-1)
+        else:
+            probs_per_est = F.softmax(logits, dim=-1)
+
         probs = probs_per_est.mean(dim=1)
-        self.val_metrics.update(probs, targets)
+        self.val_cls_metrics.update(probs, targets)
 
     def test_step(
         self,
         batch: Tuple[torch.Tensor, torch.Tensor],
         batch_idx: int,
-        dataloader_idx: int,
+        dataloader_idx: Optional[int] = 0,
     ) -> None:
         inputs, targets = batch
         logits = self.forward(inputs)
         logits = rearrange(logits, "(n b) c -> b n c", n=self.num_estimators)
-        probs_per_est = F.softmax(logits, dim=-1)
+
+        if self.binary_cls:
+            probs_per_est = torch.sigmoid(logits)
+        else:
+            probs_per_est = F.softmax(logits, dim=-1)
+
         probs = probs_per_est.mean(dim=1)
         confs, _ = probs.max(-1)
 
         if self.use_logits:
             ood_values, _ = -logits.mean(dim=1).max(dim=-1)
         elif self.use_entropy:
             ood_values = torch.special.entr(probs).sum(dim=-1).mean(dim=1)
@@ -357,50 +425,58 @@
         elif self.use_variation_ratio:
             vr_metric = VariationRatio(reduction="none", probabilistic=False)
             ood_values = vr_metric(probs_per_est.transpose(0, 1))
         else:
             ood_values = -confs
 
         if dataloader_idx == 0:
+            # squeeze if binary classification only for binary metrics
             self.test_cls_metrics.update(
-                probs,
+                probs.squeeze(-1) if self.binary_cls else probs,
                 targets,
             )
-            self.test_ood_metrics.update(ood_values, torch.zeros_like(targets))
             self.test_entropy_id(probs)
+
             self.test_id_ens_metrics.update(probs_per_est)
             self.log(
-                "test_entropy_id",
+                "hp/test_entropy_id",
                 self.test_entropy_id,
                 on_epoch=True,
                 add_dataloader_idx=False,
             )
-        else:
+
+            if self.ood_detection:
+                self.test_ood_metrics.update(
+                    ood_values, torch.zeros_like(targets)
+                )
+        elif self.ood_detection and dataloader_idx == 1:
             self.test_ood_metrics.update(ood_values, torch.ones_like(targets))
             self.test_entropy_ood(probs)
             self.test_ood_ens_metrics.update(probs_per_est)
             self.log(
-                "test_entropy_ood",
+                "hp/test_entropy_ood",
                 self.test_entropy_ood,
                 on_epoch=True,
                 add_dataloader_idx=False,
             )
 
     def test_epoch_end(
         self, outputs: Union[EPOCH_OUTPUT, List[EPOCH_OUTPUT]]
     ) -> None:
         super().test_epoch_end(outputs)
         self.log_dict(
             self.test_id_ens_metrics.compute(),
         )
-        self.log_dict(
-            self.test_ood_ens_metrics.compute(),
-        )
         self.test_id_ens_metrics.reset()
-        self.test_ood_ens_metrics.reset()
+
+        if self.ood_detection:
+            self.log_dict(
+                self.test_ood_ens_metrics.compute(),
+            )
+            self.test_ood_ens_metrics.reset()
 
     @staticmethod
     def add_model_specific_args(
         parent_parser: ArgumentParser,
     ) -> ArgumentParser:
         """Defines the routine's attributes via command-line options:
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/transforms/cutout.py` & `torch_uncertainty-0.1.3/torch_uncertainty/transforms/cutout.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/transforms/pixmix.py` & `torch_uncertainty-0.1.3/torch_uncertainty/transforms/pixmix.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,22 +15,22 @@
         b = np.float32(np.random.beta(1, beta))
     else:
         a = 1 + np.float32(np.random.beta(1, beta))
         b = -np.float32(np.random.beta(1, beta))
     return a, b
 
 
-def add(img1: Image, img2: Image, beta: float) -> Image:
+def add(img1: Image.Image, img2: Image.Image, beta: float) -> Image.Image:
     a, b = get_ab(beta)
     img1, img2 = img1 * 2 - 1, img2 * 2 - 1
     out = a * img1 + b * img2
     return (out + 1) / 2
 
 
-def multiply(img1: Image, img2: Image, beta: float) -> Image:
+def multiply(img1: Image.Image, img2: Image.Image, beta: float) -> Image.Image:
     a, b = get_ab(beta)
     img1, img2 = img1 * 2, img2 * 2
     out = (img1**a) * (img2.clip(1e-37) ** b)
     return out / 2
 
 
 # Summarize mixing operations
@@ -66,24 +66,26 @@
         self.augmentation_severity = augmentation_severity
         self.mixing_severity = mixing_severity
 
         if not all_ops:
             allowed_augmentations = [
                 aug for aug in augmentations if not aug.corruption_overlap
             ]
+        else:
+            allowed_augmentations = augmentations
 
         self.aug_instances = []
         for aug in allowed_augmentations:
             if aug == Shear or aug == Translate:
                 self.aug_instances.append(aug(axis=0))
                 self.aug_instances.append(aug(axis=1))
             else:
                 self.aug_instances.append(aug())
 
-    def __call__(self, img: Image) -> np.ndarray:
+    def __call__(self, img: Image.Image) -> np.ndarray:
         if np.random.random() < 0.5:
             mixed = self.augment_input(img)
         else:
             mixed = img
 
         for _ in range(np.random.randint(self.mixing_iterations + 1)):
             if np.random.random() < 0.5:
@@ -94,15 +96,15 @@
             mixed_op = np.random.choice(mixings)
             mixed = mixed_op(
                 np.array(mixed), np.array(aug_image_copy), self.mixing_severity
             )
             mixed = np.clip(mixed, 0, 1)
         return mixed
 
-    def _augment(self, image: Image) -> np.ndarray:
+    def _augment(self, image: Image.Image) -> np.ndarray:
         op = np.random.choice(self.aug_instances)
         if op.level_type == int:
             aug_level = self._sample_int(op.pixmix_max_level)
         else:
             aug_level = self._sample_float(op.pixmix_max_level)
         return op(image.copy(), aug_level)
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/transforms/transforms.py` & `torch_uncertainty-0.1.3/torch_uncertainty/transforms/transforms.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def forward(
         self, img: Union[Tensor, Image.Image], level: float
     ) -> Union[Tensor, Image.Image]:
         if (
             self.random_direction and np.random.uniform() > 0.5
         ):  # coverage: ignore
-            level = -level  # coverage: ignore
+            level = -level
         return F.rotate(
             img,
             level,
             interpolation=self.interpolation,
             expand=self.expand,
             center=self.center,
             fill=self.fill,
@@ -124,15 +124,15 @@
 
     def forward(
         self, img: Union[Tensor, Image.Image], level: float
     ) -> Union[Tensor, Image.Image]:
         if (
             self.random_direction and np.random.uniform() > 0.5
         ):  # coverage: ignore
-            level = -level  # coverage: ignore
+            level = -level
         shear = [0, 0]
         shear[self.axis] = level
         return F.affine(
             img,
             angle=0,
             scale=1.0,
             shear=shear,
@@ -167,15 +167,15 @@
 
     def forward(
         self, img: Union[Tensor, Image.Image], level: float
     ) -> Union[Tensor, Image.Image]:
         if (
             self.random_direction and np.random.uniform() > 0.5
         ):  # coverage: ignore
-            level = -level  # coverage: ignore
+            level = -level
         translate = [0, 0]
         translate[self.axis] = level
         return F.affine(
             img,
             angle=0,
             scale=1.0,
             shear=[0, 0],
```

### Comparing `torch_uncertainty-0.1.2/torch_uncertainty/utils/checkpoints.py` & `torch_uncertainty-0.1.3/torch_uncertainty/utils/checkpoints.py`

 * *Files identical despite different names*

### Comparing `torch_uncertainty-0.1.2/setup.py` & `torch_uncertainty-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['torch_uncertainty',
  'torch_uncertainty.baselines',
  'torch_uncertainty.baselines.classification',
+ 'torch_uncertainty.baselines.regression',
  'torch_uncertainty.baselines.utils',
  'torch_uncertainty.datamodules',
  'torch_uncertainty.datasets',
  'torch_uncertainty.datasets.cifar',
  'torch_uncertainty.datasets.imagenet',
  'torch_uncertainty.layers',
+ 'torch_uncertainty.layers.bayesian_layers',
  'torch_uncertainty.metrics',
  'torch_uncertainty.models',
  'torch_uncertainty.models.resnet',
+ 'torch_uncertainty.models.vgg',
  'torch_uncertainty.models.wideresnet',
  'torch_uncertainty.post_processing',
  'torch_uncertainty.routines',
  'torch_uncertainty.transforms',
  'torch_uncertainty.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['einops>=0.6.0,<0.7.0',
+['einops>=0.6.0',
  'huggingface-hub>=0.14.1,<0.15.0',
+ 'pandas>=2.0.3,<3.0.0',
  'pytorch-lightning>=1.9.0,<2.0.0',
  'scipy>=1.10.0,<2.0.0',
- 'tensorboard>=2.11.2,<3.0.0',
- 'timm>=0.6.12,<0.7.0',
- 'torchinfo>=1.7.1,<2.0.0',
- 'torchvision>=0.14.1,<0.15.0']
+ 'tensorboard>=2.11.2',
+ 'timm>=0.6.12',
+ 'torchinfo>=1.7.1']
 
 setup_kwargs = {
     'name': 'torch-uncertainty',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques.',
-    'long_description': '<div align="center">\n\n![Torch Uncertainty Logo](https://github.com/ENSTA-U2IS/torch-uncertainty/blob/main/docs/source/_static/images/torch_uncertainty.png)\n\n[![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty)\n[![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml)\n[![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/)\n[![Code Coverage](https://codecov.io/github/ENSTA-U2IS/torch-uncertainty/coverage.svg?branch=master)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n</div>\n\n_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.\n\n:construction: _TorchUncertainty_ is in early development :construction: - expect massive changes but do reach out to us and contribute if you are interested by the project!\n\n---\n\nThis package provides a multi-level API, including:\n\n- ready-to-train baselines on research datasets, such as ImageNet and CIFAR\n- baselines available for training on your datasets\n- [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR (work in progress 🚧).\n- layers available for use in your networks\n- post-processing methods such as temperature scaling\n\n## Installation\n\nThe package can be installed from PyPI:\n\n```sh\npip install torch-uncertainty\n```\n\nTo contribute, install the package from source following the instructions of the [dedicated page](https://torch-uncertainty.github.io/installation.html) in the documentation and activate the pre-commit hooks with `pre-commit install`.\n\n## Getting Started and Documentation\n\nPlease find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).\n\nA quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).\n\n## Implemented methods\n\n### Baselines\n\nTo date, the following baselines are implemented:\n\n- Deep Ensembles\n- BatchEnsemble\n- Masksembles\n- Packed-Ensembles (see [blog post](https://medium.com/@adrien.lafage/make-your-neural-networks-more-reliable-with-packed-ensembles-7ad0b737a873))\n\n### Post-processing methods\n\nTo date, the following post-processing methods are implemented:\n\n- Temperature scaling\n\n## Tutorials\n\n## Awesome Uncertainty repositories\n\nYou may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).\n\n## Other References\n\nThis package also contains the official implementation of Packed-Ensembles.\n\nIf you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):\n\n```text\n@inproceedings{laurent2023packed,\n    title={Packed-Ensembles for Efficient Uncertainty Estimation},\n    author={Laurent, Olivier and Lafage, Adrien and Tartaglione, Enzo and Daniel, Geoffrey and Martinez, Jean-Marc and Bursuc, Andrei and Franchi, Gianni},\n    booktitle={ICLR},\n    year={2023}\n}\n```\n',
+    'long_description': '<div align="center">\n\n![Torch Uncertainty Logo](https://github.com/ENSTA-U2IS/torch-uncertainty/blob/main/docs/source/_static/images/torch_uncertainty.png)\n\n[![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty)\n[![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml)\n[![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/)\n[![Code Coverage](https://codecov.io/github/ENSTA-U2IS/torch-uncertainty/coverage.svg?branch=master)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n</div>\n\n_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It aims at including as many methods as possible, so reach out to add yours!\n\n:construction: _TorchUncertainty_ is in early development :construction: - expect massive changes but do reach out to us and contribute if you are interested by the project!\n\n---\n\nThis package provides a multi-level API, including:\n\n- ready-to-train baselines on research datasets, such as ImageNet and CIFAR\n- baselines available for training on your datasets\n- [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR (work in progress 🚧).\n- layers available for use in your networks\n- scikit-learn style post-processing methods such as Temperature Scaling\n\nSee the [Reference page](https://torch-uncertainty.github.io/references.html) or the [API reference](https://torch-uncertainty.github.io/api.html) for a more exhaustive list of the implemented methods, datasets, metrics, etc.\n\n## Installation\n\nInstall the desired pytorch version in your environment. Then, the package can be installed from PyPI:\n\n```sh\npip install torch-uncertainty\n```\n\nIf you aim to contribute (thank you!), have a look at the [contribution page](https://torch-uncertainty.github.io/contributing.html).\n\n## Getting Started and Documentation\n\nPlease find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).\n\nA quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).\n\n## Implemented methods\n\n### Baselines\n\nTo date, the following baselines are implemented:\n\n- Deep Ensembles\n- BatchEnsemble\n- Masksembles\n- Packed-Ensembles (see [blog post](https://medium.com/@adrien.lafage/make-your-neural-networks-more-reliable-with-packed-ensembles-7ad0b737a873))\n- Bayesian Neural Networks\n\n### Post-processing methods\n\nTo date, the following post-processing methods are implemented:\n\n- Temperature scaling\n\n## Tutorials\n\n## Awesome Uncertainty repositories\n\nYou may find a lot of papers about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).\n\n## Other References\n\nThis package also contains the official implementation of Packed-Ensembles.\n\nIf you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):\n\n```text\n@inproceedings{laurent2023packed,\n    title={Packed-Ensembles for Efficient Uncertainty Estimation},\n    author={Laurent, Olivier and Lafage, Adrien and Tartaglione, Enzo and Daniel, Geoffrey and Martinez, Jean-Marc and Bursuc, Andrei and Franchi, Gianni},\n    booktitle={ICLR},\n    year={2023}\n}\n```\n',
     'author': 'ENSTA U2IS',
     'author_email': 'olivier.laurent@ensta-paris.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `torch_uncertainty-0.1.2/PKG-INFO` & `torch_uncertainty-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 Metadata-Version: 2.1
 Name: torch-uncertainty
-Version: 0.1.2
+Version: 0.1.3
 Summary: A PyTorch Library for benchmarking and leveraging efficient predictive uncertainty quantification techniques.
 License: Apache-2.0
 Keywords: deep-learning,pytorch,uncertainty,ensembles,uncertainty-quantification,predictive-uncertainty,reliable-ai,deep-learning-uncertainty
 Author: ENSTA U2IS
 Author-email: olivier.laurent@ensta-paris.fr
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: einops (>=0.6.0,<0.7.0)
+Requires-Dist: einops (>=0.6.0)
 Requires-Dist: huggingface-hub (>=0.14.1,<0.15.0)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pytorch-lightning (>=1.9.0,<2.0.0)
 Requires-Dist: scipy (>=1.10.0,<2.0.0)
-Requires-Dist: tensorboard (>=2.11.2,<3.0.0)
-Requires-Dist: timm (>=0.6.12,<0.7.0)
-Requires-Dist: torchinfo (>=1.7.1,<2.0.0)
-Requires-Dist: torchvision (>=0.14.1,<0.15.0)
+Requires-Dist: tensorboard (>=2.11.2)
+Requires-Dist: timm (>=0.6.12)
+Requires-Dist: torchinfo (>=1.7.1)
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 ![Torch Uncertainty Logo](https://github.com/ENSTA-U2IS/torch-uncertainty/blob/main/docs/source/_static/images/torch_uncertainty.png)
 
 [![pypi](https://img.shields.io/pypi/v/torch_uncertainty.svg)](https://pypi.python.org/pypi/torch_uncertainty)
 [![tests](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml/badge.svg?branch=main&event=push)](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/run-tests.yml)
 [![Docs](https://github.com/ENSTA-U2IS/torch-uncertainty/actions/workflows/build-docs.yml/badge.svg)](https://torch-uncertainty.github.io/)
 [![Code Coverage](https://codecov.io/github/ENSTA-U2IS/torch-uncertainty/coverage.svg?branch=master)](https://codecov.io/gh/ENSTA-U2IS/torch-uncertainty)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)
 </div>
 
-_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It is based on PyTorch Lightning to handle multi-GPU training and inference and automatic logging through tensorboard.
+_TorchUncertainty_ is a package designed to help you leverage uncertainty quantification techniques and make your neural networks more reliable. It aims at including as many methods as possible, so reach out to add yours!
 
 :construction: _TorchUncertainty_ is in early development :construction: - expect massive changes but do reach out to us and contribute if you are interested by the project!
 
 ---
 
 This package provides a multi-level API, including:
 
 - ready-to-train baselines on research datasets, such as ImageNet and CIFAR
 - baselines available for training on your datasets
 - [pretrained weights](https://huggingface.co/torch-uncertainty) for these baselines on ImageNet and CIFAR (work in progress 🚧).
 - layers available for use in your networks
-- post-processing methods such as temperature scaling
+- scikit-learn style post-processing methods such as Temperature Scaling
+
+See the [Reference page](https://torch-uncertainty.github.io/references.html) or the [API reference](https://torch-uncertainty.github.io/api.html) for a more exhaustive list of the implemented methods, datasets, metrics, etc.
 
 ## Installation
 
-The package can be installed from PyPI:
+Install the desired pytorch version in your environment. Then, the package can be installed from PyPI:
 
 ```sh
 pip install torch-uncertainty
 ```
 
-To contribute, install the package from source following the instructions of the [dedicated page](https://torch-uncertainty.github.io/installation.html) in the documentation and activate the pre-commit hooks with `pre-commit install`.
+If you aim to contribute (thank you!), have a look at the [contribution page](https://torch-uncertainty.github.io/contributing.html).
 
 ## Getting Started and Documentation
 
 Please find the documentation at [torch-uncertainty.github.io](https://torch-uncertainty.github.io).
 
 A quickstart is available at [torch-uncertainty.github.io/quickstart](https://torch-uncertainty.github.io/quickstart.html).
 
@@ -69,26 +71,27 @@
 
 To date, the following baselines are implemented:
 
 - Deep Ensembles
 - BatchEnsemble
 - Masksembles
 - Packed-Ensembles (see [blog post](https://medium.com/@adrien.lafage/make-your-neural-networks-more-reliable-with-packed-ensembles-7ad0b737a873))
+- Bayesian Neural Networks
 
 ### Post-processing methods
 
 To date, the following post-processing methods are implemented:
 
 - Temperature scaling
 
 ## Tutorials
 
 ## Awesome Uncertainty repositories
 
-You may find a lot of information about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).
+You may find a lot of papers about modern uncertainty estimation techniques on the [Awesome Uncertainty in Deep Learning](https://github.com/ENSTA-U2IS/awesome-uncertainty-deeplearning).
 
 ## Other References
 
 This package also contains the official implementation of Packed-Ensembles.
 
 If you find the corresponding models interesting, please consider citing our [paper](https://arxiv.org/abs/2210.09184):
```

