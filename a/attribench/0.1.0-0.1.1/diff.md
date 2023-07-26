# Comparing `tmp/attribench-0.1.0.tar.gz` & `tmp/attribench-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "attribench-0.1.0.tar", last modified: Wed Jul 26 09:43:42 2023, max compression
+gzip compressed data, was "attribench-0.1.1.tar", last modified: Wed Jul 26 13:18:49 2023, max compression
```

## Comparing `attribench-0.1.0.tar` & `attribench-0.1.1.tar`

### file list

```diff
@@ -1,299 +1,296 @@
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.356729 attribench-0.1.0/
--rw-rw-r--   0 arne      (1000) arne      (1000)     1068 2023-06-12 12:11:57.000000 attribench-0.1.0/LICENSE
--rw-rw-r--   0 arne      (1000) arne      (1000)     2190 2023-07-26 09:43:42.356729 attribench-0.1.0/PKG-INFO
--rw-rw-r--   0 arne      (1000) arne      (1000)      260 2023-07-26 09:26:20.000000 attribench-0.1.0/README.rst
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.328729 attribench-0.1.0/attribench/
--rw-rw-r--   0 arne      (1000) arne      (1000)      177 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      294 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/_activation_fns.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1240 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/_attribution_method.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2808 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/_method_factory.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1274 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/_model_factory.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1528 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/_segmentation.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2866 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/_stat.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.328729 attribench-0.1.0/attribench/data/
--rw-rw-r--   0 arne      (1000) arne      (1000)      323 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      777 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/_index_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      189 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/_typing.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/data/attributions_dataset/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/attributions_dataset/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)    11835 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/attributions_dataset/_attributions_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1216 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/attributions_dataset/_attributions_dataset_writer.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/data/hdf5_dataset/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/hdf5_dataset/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1428 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/hdf5_dataset/_hdf5_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2323 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/hdf5_dataset/_hdf5_dataset_writer.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/data/nd_array_tree/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/nd_array_tree/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     6081 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/nd_array_tree/_nd_array_tree.py
--rw-rw-r--   0 arne      (1000) arne      (1000)    13407 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/data/nd_array_tree/_random_access_nd_array_tree.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/distributed/
--rw-rw-r--   0 arne      (1000) arne      (1000)      198 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5859 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/_compute_attributions.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2851 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/_distributed_computation.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      907 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/_distributed_sampler.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      318 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/_message.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5584 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/_select_samples.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5287 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/_train_adversarial_patches.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2033 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/distributed/metrics/
--rw-rw-r--   0 arne      (1000) arne      (1000)      518 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3098 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/_metric.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3628 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/_metric_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/distributed/metrics/deletion/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/deletion/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4718 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/deletion/_deletion.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1410 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/deletion/_deletion_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/distributed/metrics/impact_coverage/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/impact_coverage/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3879 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/impact_coverage/_impact_coverage.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1966 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/impact_coverage/_impact_coverage_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/distributed/metrics/infidelity/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/infidelity/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4663 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/infidelity/_infidelity.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1526 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/infidelity/_infidelity_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.332729 attribench-0.1.0/attribench/distributed/metrics/insertion/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/insertion/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4749 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/insertion/_insertion.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/distributed/metrics/irof/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/irof/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4438 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/irof/_irof.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1470 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/irof/_irof_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/distributed/metrics/max_sensitivity/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/max_sensitivity/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3931 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/max_sensitivity/_max_sensitivity.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1524 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/max_sensitivity/_max_sensitivity_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/distributed/metrics/minimal_subset/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/minimal_subset/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3958 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/minimal_subset/_minimal_subset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1179 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/minimal_subset/_minimal_subset_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/distributed/metrics/parameter_randomization/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/parameter_randomization/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3547 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/parameter_randomization/_parameter_randomization.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1701 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/parameter_randomization/_parameter_randomization_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/distributed/metrics/sensitivity_n/
--rw-rw-r--   0 arne      (1000) arne      (1000)       40 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/sensitivity_n/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5437 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/sensitivity_n/_sensitivity_n.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2035 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/distributed/metrics/sensitivity_n/_sensitivity_n_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/functional/
--rw-rw-r--   0 arne      (1000) arne      (1000)      165 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3036 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/_compute_attributions.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3270 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/_select_samples.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     7102 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/_train_adversarial_patches.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/functional/metrics/
--rw-rw-r--   0 arne      (1000) arne      (1000)      361 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     8740 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/_impact_coverage.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4216 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/_insertion.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4617 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/_irof.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4929 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/_max_sensitivity.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5262 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/_parameter_randomization.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/functional/metrics/deletion/
--rw-rw-r--   0 arne      (1000) arne      (1000)       31 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/deletion/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2751 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/deletion/_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4504 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/deletion/_deletion.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      877 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/deletion/_get_predictions.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/functional/metrics/infidelity/
--rw-rw-r--   0 arne      (1000) arne      (1000)      253 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/infidelity/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     8782 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/infidelity/_infidelity.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3964 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/infidelity/_perturbation_generator.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.336729 attribench-0.1.0/attribench/functional/metrics/minimal_subset/
--rw-rw-r--   0 arne      (1000) arne      (1000)       43 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/minimal_subset/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1663 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/minimal_subset/_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5525 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/minimal_subset/_minimal_subset.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.340729 attribench-0.1.0/attribench/functional/metrics/sensitivity_n/
--rw-rw-r--   0 arne      (1000) arne      (1000)       41 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/sensitivity_n/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2248 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/sensitivity_n/_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)    10175 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/functional/metrics/sensitivity_n/_sensitivity_n.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.340729 attribench-0.1.0/attribench/masking/
--rw-rw-r--   0 arne      (1000) arne      (1000)       69 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4211 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/_masker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.340729 attribench-0.1.0/attribench/masking/image/
--rw-rw-r--   0 arne      (1000) arne      (1000)      269 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/image/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1866 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/image/_blurring_image_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      809 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/image/_constant_image_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)    12086 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/image/_image_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      830 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/image/_random_image_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      821 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/image/_sample_average_image_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2111 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/masking/tabular_masker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.340729 attribench-0.1.0/attribench/plot/
--rw-rw-r--   0 arne      (1000) arne      (1000)      429 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2415 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_cles_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2209 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_cluster_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2715 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_convergence_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5146 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_correlations.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1384 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_krippendorff_alpha_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4183 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_lib.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2089 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_mad_ratio_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      886 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2716 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_wilcoxon_barplot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2722 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/plot/_wilcoxon_summary_plot.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.340729 attribench-0.1.0/attribench/result/
--rw-rw-r--   0 arne      (1000) arne      (1000)      537 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      430 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_batch_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5982 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_deletion_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      588 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_grouped_batch_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      865 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_grouped_metric_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1934 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_impact_coverage_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2993 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_infidelity_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1369 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_insertion_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1903 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_max_sensitivity_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     6017 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_metric_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3712 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_minimal_subset_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1948 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_parameter_randomization_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3590 2023-07-26 09:26:20.000000 attribench-0.1.0/attribench/result/_sensitivity_n_result.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.352729 attribench-0.1.0/attribench.egg-info/
--rw-rw-r--   0 arne      (1000) arne      (1000)     2190 2023-07-26 09:43:42.000000 attribench-0.1.0/attribench.egg-info/PKG-INFO
--rw-rw-r--   0 arne      (1000) arne      (1000)    17777 2023-07-26 09:43:42.000000 attribench-0.1.0/attribench.egg-info/SOURCES.txt
--rw-rw-r--   0 arne      (1000) arne      (1000)        1 2023-07-26 09:43:42.000000 attribench-0.1.0/attribench.egg-info/dependency_links.txt
--rw-rw-r--   0 arne      (1000) arne      (1000)      240 2023-07-26 09:43:42.000000 attribench-0.1.0/attribench.egg-info/requires.txt
--rw-rw-r--   0 arne      (1000) arne      (1000)       11 2023-07-26 09:43:42.000000 attribench-0.1.0/attribench.egg-info/top_level.txt
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.324729 attribench-0.1.0/build/
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.328729 attribench-0.1.0/build/lib/
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/
--rw-rw-r--   0 arne      (1000) arne      (1000)      154 2023-07-18 08:49:55.000000 attribench-0.1.0/build/lib/attribench/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      294 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/_activation_fns.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1240 2023-07-18 08:49:02.000000 attribench-0.1.0/build/lib/attribench/_attribution_method.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2808 2023-07-19 12:11:02.000000 attribench-0.1.0/build/lib/attribench/_method_factory.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1274 2023-07-18 08:52:22.000000 attribench-0.1.0/build/lib/attribench/_model_factory.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1528 2023-07-19 14:49:06.000000 attribench-0.1.0/build/lib/attribench/_segmentation.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2866 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/_stat.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/data/
--rw-rw-r--   0 arne      (1000) arne      (1000)      323 2023-06-14 14:07:03.000000 attribench-0.1.0/build/lib/attribench/data/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      777 2023-07-19 15:13:56.000000 attribench-0.1.0/build/lib/attribench/data/_index_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      189 2023-07-17 08:32:44.000000 attribench-0.1.0/build/lib/attribench/data/_typing.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/data/attributions_dataset/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 14:05:47.000000 attribench-0.1.0/build/lib/attribench/data/attributions_dataset/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)    11835 2023-07-19 15:32:55.000000 attribench-0.1.0/build/lib/attribench/data/attributions_dataset/_attributions_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1216 2023-07-19 13:13:40.000000 attribench-0.1.0/build/lib/attribench/data/attributions_dataset/_attributions_dataset_writer.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/data/hdf5_dataset/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 14:05:51.000000 attribench-0.1.0/build/lib/attribench/data/hdf5_dataset/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1428 2023-07-18 08:56:37.000000 attribench-0.1.0/build/lib/attribench/data/hdf5_dataset/_hdf5_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2323 2023-07-19 13:12:24.000000 attribench-0.1.0/build/lib/attribench/data/hdf5_dataset/_hdf5_dataset_writer.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/data/nd_array_tree/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 14:05:56.000000 attribench-0.1.0/build/lib/attribench/data/nd_array_tree/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     6081 2023-07-15 15:14:55.000000 attribench-0.1.0/build/lib/attribench/data/nd_array_tree/_nd_array_tree.py
--rw-rw-r--   0 arne      (1000) arne      (1000)    13407 2023-07-15 15:29:50.000000 attribench-0.1.0/build/lib/attribench/data/nd_array_tree/_random_access_nd_array_tree.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/distributed/
--rw-rw-r--   0 arne      (1000) arne      (1000)      198 2023-06-15 05:04:31.000000 attribench-0.1.0/build/lib/attribench/distributed/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5859 2023-07-19 13:14:15.000000 attribench-0.1.0/build/lib/attribench/distributed/_compute_attributions.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2851 2023-07-21 06:47:03.000000 attribench-0.1.0/build/lib/attribench/distributed/_distributed_computation.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      907 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/distributed/_distributed_sampler.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      318 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/distributed/_message.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5584 2023-07-19 13:08:34.000000 attribench-0.1.0/build/lib/attribench/distributed/_select_samples.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5287 2023-07-18 08:56:52.000000 attribench-0.1.0/build/lib/attribench/distributed/_train_adversarial_patches.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2033 2023-07-17 06:25:18.000000 attribench-0.1.0/build/lib/attribench/distributed/_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/distributed/metrics/
--rw-rw-r--   0 arne      (1000) arne      (1000)      518 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3098 2023-07-21 13:33:42.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/_metric.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3628 2023-07-19 15:18:56.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/_metric_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 09:44:50.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4718 2023-07-21 06:15:58.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/_deletion.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1410 2023-07-17 13:40:15.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/_deletion_worker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4706 2023-06-15 12:07:07.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/_insertion.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     7166 2023-07-16 07:54:04.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/_irof.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/distributed/metrics/impact_coverage/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 09:49:05.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/impact_coverage/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3879 2023-07-21 06:23:14.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/impact_coverage/_impact_coverage.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1966 2023-07-17 08:55:17.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/impact_coverage/_impact_coverage_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/distributed/metrics/infidelity/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-16 07:17:59.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/infidelity/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4663 2023-07-21 06:18:44.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/infidelity/_infidelity.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1526 2023-07-19 15:18:41.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/infidelity/_infidelity_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/distributed/metrics/max_sensitivity/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 12:27:30.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/max_sensitivity/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3931 2023-07-21 06:22:42.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/max_sensitivity/_max_sensitivity.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1524 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/max_sensitivity/_max_sensitivity_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.344729 attribench-0.1.0/build/lib/attribench/distributed/metrics/minimal_subset/
--rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 12:30:21.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/minimal_subset/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3958 2023-07-21 06:21:52.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/minimal_subset/_minimal_subset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1179 2023-07-16 08:03:42.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/minimal_subset/_minimal_subset_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.348729 attribench-0.1.0/build/lib/attribench/distributed/metrics/sensitivity_n/
--rw-rw-r--   0 arne      (1000) arne      (1000)       40 2023-07-09 09:02:45.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/sensitivity_n/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5437 2023-07-21 06:20:48.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/sensitivity_n/_sensitivity_n.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2035 2023-07-19 15:32:37.000000 attribench-0.1.0/build/lib/attribench/distributed/metrics/sensitivity_n/_sensitivity_n_worker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.348729 attribench-0.1.0/build/lib/attribench/functional/
--rw-rw-r--   0 arne      (1000) arne      (1000)      165 2023-06-15 07:07:46.000000 attribench-0.1.0/build/lib/attribench/functional/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3036 2023-07-19 13:06:31.000000 attribench-0.1.0/build/lib/attribench/functional/_compute_attributions.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3270 2023-07-19 11:45:05.000000 attribench-0.1.0/build/lib/attribench/functional/_select_samples.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     7102 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/functional/_train_adversarial_patches.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.348729 attribench-0.1.0/build/lib/attribench/functional/metrics/
--rw-rw-r--   0 arne      (1000) arne      (1000)      361 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     8740 2023-07-21 06:37:24.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/_impact_coverage.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4216 2023-07-21 06:28:11.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/_insertion.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4617 2023-07-21 06:29:11.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/_irof.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4929 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/_max_sensitivity.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5262 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/_parameter_randomization.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.348729 attribench-0.1.0/build/lib/attribench/functional/metrics/deletion/
--rw-rw-r--   0 arne      (1000) arne      (1000)       31 2023-06-15 07:51:41.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/deletion/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2751 2023-07-17 13:43:40.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/deletion/_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4504 2023-07-21 13:21:48.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/deletion/_deletion.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      877 2023-06-15 08:15:06.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/deletion/_get_predictions.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.348729 attribench-0.1.0/build/lib/attribench/functional/metrics/infidelity/
--rw-rw-r--   0 arne      (1000) arne      (1000)      253 2023-07-19 14:12:51.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/infidelity/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     8782 2023-07-21 06:30:12.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/infidelity/_infidelity.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3964 2023-06-16 07:19:46.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/infidelity/_perturbation_generator.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.348729 attribench-0.1.0/build/lib/attribench/functional/metrics/minimal_subset/
--rw-rw-r--   0 arne      (1000) arne      (1000)       43 2023-06-16 09:37:14.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/minimal_subset/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1663 2023-07-21 06:34:50.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/minimal_subset/_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5525 2023-07-21 06:35:55.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/minimal_subset/_minimal_subset.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.348729 attribench-0.1.0/build/lib/attribench/functional/metrics/sensitivity_n/
--rw-rw-r--   0 arne      (1000) arne      (1000)       41 2023-07-07 12:54:55.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/sensitivity_n/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2248 2023-07-17 14:18:11.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/sensitivity_n/_dataset.py
--rw-rw-r--   0 arne      (1000) arne      (1000)    10175 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/functional/metrics/sensitivity_n/_sensitivity_n.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.348729 attribench-0.1.0/build/lib/attribench/masking/
--rw-rw-r--   0 arne      (1000) arne      (1000)       69 2023-07-17 13:46:49.000000 attribench-0.1.0/build/lib/attribench/masking/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4211 2023-07-18 08:57:40.000000 attribench-0.1.0/build/lib/attribench/masking/_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1110 2023-07-17 12:17:39.000000 attribench-0.1.0/build/lib/attribench/masking/blurring_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      401 2023-07-17 12:17:39.000000 attribench-0.1.0/build/lib/attribench/masking/constant_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     8617 2023-06-15 11:37:49.000000 attribench-0.1.0/build/lib/attribench/masking/image_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1476 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/masking/masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      425 2023-07-17 12:17:39.000000 attribench-0.1.0/build/lib/attribench/masking/random_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      477 2023-07-17 12:17:39.000000 attribench-0.1.0/build/lib/attribench/masking/sample_average_masker.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2111 2023-07-17 13:39:10.000000 attribench-0.1.0/build/lib/attribench/masking/tabular_masker.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.352729 attribench-0.1.0/build/lib/attribench/plot/
--rw-rw-r--   0 arne      (1000) arne      (1000)      429 2023-07-21 07:44:01.000000 attribench-0.1.0/build/lib/attribench/plot/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2415 2023-07-18 07:40:27.000000 attribench-0.1.0/build/lib/attribench/plot/_cles_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2209 2023-07-18 07:42:07.000000 attribench-0.1.0/build/lib/attribench/plot/_cluster_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2715 2023-07-18 08:58:09.000000 attribench-0.1.0/build/lib/attribench/plot/_convergence_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5146 2023-07-18 07:25:08.000000 attribench-0.1.0/build/lib/attribench/plot/_correlations.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1384 2023-07-18 07:27:47.000000 attribench-0.1.0/build/lib/attribench/plot/_krippendorff_alpha_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4183 2023-07-17 15:26:00.000000 attribench-0.1.0/build/lib/attribench/plot/_lib.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2089 2023-07-18 07:36:12.000000 attribench-0.1.0/build/lib/attribench/plot/_mad_ratio_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      886 2023-07-18 08:58:13.000000 attribench-0.1.0/build/lib/attribench/plot/_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2716 2023-07-18 07:37:09.000000 attribench-0.1.0/build/lib/attribench/plot/_wilcoxon_barplot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2722 2023-07-17 15:35:42.000000 attribench-0.1.0/build/lib/attribench/plot/_wilcoxon_summary_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1157 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/plot/cles_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1631 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/plot/cluster_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1445 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/plot/convergence_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2416 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/plot/correlations.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      866 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/plot/krippendorff_alpha.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     4844 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/plot/lib.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1589 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/attribench/plot/mad_ratio_plot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1185 2023-07-17 14:25:06.000000 attribench-0.1.0/build/lib/attribench/plot/wilcoxon_barplot.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1565 2023-07-17 14:25:06.000000 attribench-0.1.0/build/lib/attribench/plot/wilcoxon_summary_plot.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.352729 attribench-0.1.0/build/lib/attribench/result/
--rw-rw-r--   0 arne      (1000) arne      (1000)      537 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/result/__init__.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      430 2023-07-13 14:54:39.000000 attribench-0.1.0/build/lib/attribench/result/_batch_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     5982 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/result/_deletion_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      588 2023-07-13 14:52:59.000000 attribench-0.1.0/build/lib/attribench/result/_grouped_batch_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)      865 2023-07-13 14:51:58.000000 attribench-0.1.0/build/lib/attribench/result/_grouped_metric_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1934 2023-07-18 08:58:20.000000 attribench-0.1.0/build/lib/attribench/result/_impact_coverage_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     2993 2023-07-18 08:58:26.000000 attribench-0.1.0/build/lib/attribench/result/_infidelity_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1369 2023-07-14 06:15:54.000000 attribench-0.1.0/build/lib/attribench/result/_insertion_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1903 2023-07-18 08:58:30.000000 attribench-0.1.0/build/lib/attribench/result/_max_sensitivity_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     6017 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/result/_metric_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3712 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/result/_minimal_subset_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1948 2023-07-26 07:10:26.000000 attribench-0.1.0/build/lib/attribench/result/_parameter_randomization_result.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     3590 2023-07-21 13:29:34.000000 attribench-0.1.0/build/lib/attribench/result/_sensitivity_n_result.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.328729 attribench-0.1.0/build/lib/docs/
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.352729 attribench-0.1.0/build/lib/docs/source/
--rw-rw-r--   0 arne      (1000) arne      (1000)     2605 2023-07-18 08:55:42.000000 attribench-0.1.0/build/lib/docs/source/conf.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.352729 attribench-0.1.0/build/lib/tests/
--rw-rw-r--   0 arne      (1000) arne      (1000)      117 2023-06-12 12:11:57.000000 attribench-0.1.0/build/lib/tests/test.py
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.328729 attribench-0.1.0/docs/
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.352729 attribench-0.1.0/docs/source/
--rw-rw-r--   0 arne      (1000) arne      (1000)     2605 2023-07-26 09:26:20.000000 attribench-0.1.0/docs/source/conf.py
--rw-rw-r--   0 arne      (1000) arne      (1000)     1621 2023-07-26 09:43:32.000000 attribench-0.1.0/pyproject.toml
--rw-rw-r--   0 arne      (1000) arne      (1000)       38 2023-07-26 09:43:42.356729 attribench-0.1.0/setup.cfg
-drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 09:43:42.352729 attribench-0.1.0/tests/
--rw-rw-r--   0 arne      (1000) arne      (1000)      117 2023-06-12 12:11:57.000000 attribench-0.1.0/tests/test.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.586608 attribench-0.1.1/
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1068 2023-06-12 12:11:57.000000 attribench-0.1.1/LICENSE
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2926 2023-07-26 13:18:49.586608 attribench-0.1.1/PKG-INFO
+-rw-rw-r--   0 arne      (1000) arne      (1000)      975 2023-07-26 12:33:24.000000 attribench-0.1.1/README.rst
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.538608 attribench-0.1.1/attribench/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      177 2023-07-26 09:48:11.000000 attribench-0.1.1/attribench/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      294 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/_activation_fns.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1240 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/_attribution_method.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2808 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/_method_factory.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1274 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/_model_factory.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1528 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/_segmentation.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2866 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/_stat.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.538608 attribench-0.1.1/attribench/data/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      323 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      777 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/_index_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      189 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/_typing.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/data/attributions_dataset/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/attributions_dataset/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)    11835 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/attributions_dataset/_attributions_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1216 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/attributions_dataset/_attributions_dataset_writer.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/data/hdf5_dataset/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/hdf5_dataset/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1428 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/hdf5_dataset/_hdf5_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2323 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/hdf5_dataset/_hdf5_dataset_writer.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/data/nd_array_tree/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/nd_array_tree/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     6081 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/nd_array_tree/_nd_array_tree.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)    13407 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/data/nd_array_tree/_random_access_nd_array_tree.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/distributed/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      198 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5859 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/_compute_attributions.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2851 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/_distributed_computation.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      907 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/_distributed_sampler.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      318 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/_message.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5584 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/_select_samples.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5287 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/_train_adversarial_patches.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2033 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/distributed/metrics/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      518 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3098 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/_metric.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3628 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/_metric_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/distributed/metrics/deletion/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/deletion/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4718 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/deletion/_deletion.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1410 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/deletion/_deletion_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/distributed/metrics/impact_coverage/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/impact_coverage/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3879 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/impact_coverage/_impact_coverage.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1966 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/impact_coverage/_impact_coverage_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/distributed/metrics/infidelity/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/infidelity/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4663 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/infidelity/_infidelity.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1526 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/infidelity/_infidelity_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.542608 attribench-0.1.1/attribench/distributed/metrics/insertion/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/insertion/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4749 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/insertion/_insertion.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.546608 attribench-0.1.1/attribench/distributed/metrics/irof/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/irof/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4438 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/irof/_irof.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1470 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/irof/_irof_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.546608 attribench-0.1.1/attribench/distributed/metrics/max_sensitivity/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/max_sensitivity/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3931 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/max_sensitivity/_max_sensitivity.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1524 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/max_sensitivity/_max_sensitivity_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.546608 attribench-0.1.1/attribench/distributed/metrics/minimal_subset/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/minimal_subset/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3958 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/minimal_subset/_minimal_subset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1179 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/minimal_subset/_minimal_subset_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.546608 attribench-0.1.1/attribench/distributed/metrics/parameter_randomization/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/parameter_randomization/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3547 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/parameter_randomization/_parameter_randomization.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1701 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/parameter_randomization/_parameter_randomization_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.546608 attribench-0.1.1/attribench/distributed/metrics/sensitivity_n/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       40 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/sensitivity_n/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5437 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/sensitivity_n/_sensitivity_n.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2035 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/distributed/metrics/sensitivity_n/_sensitivity_n_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.546608 attribench-0.1.1/attribench/functional/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      165 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3036 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/_compute_attributions.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3270 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/_select_samples.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     7102 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/_train_adversarial_patches.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.550608 attribench-0.1.1/attribench/functional/metrics/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      361 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     8740 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/_impact_coverage.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4216 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/_insertion.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4617 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/_irof.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4929 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/_max_sensitivity.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5262 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/_parameter_randomization.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.550608 attribench-0.1.1/attribench/functional/metrics/deletion/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       31 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/deletion/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2751 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/deletion/_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4504 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/deletion/_deletion.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      877 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/deletion/_get_predictions.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.550608 attribench-0.1.1/attribench/functional/metrics/infidelity/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      253 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/infidelity/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     8782 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/infidelity/_infidelity.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3964 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/infidelity/_perturbation_generator.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.550608 attribench-0.1.1/attribench/functional/metrics/minimal_subset/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       43 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/minimal_subset/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1663 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/minimal_subset/_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5525 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/minimal_subset/_minimal_subset.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.550608 attribench-0.1.1/attribench/functional/metrics/sensitivity_n/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       41 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/sensitivity_n/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2248 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/sensitivity_n/_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)    10175 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/functional/metrics/sensitivity_n/_sensitivity_n.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.550608 attribench-0.1.1/attribench/masking/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       69 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4211 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/_masker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.554608 attribench-0.1.1/attribench/masking/image/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      269 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/image/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1866 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/image/_blurring_image_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      809 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/image/_constant_image_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)    12086 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/image/_image_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      830 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/image/_random_image_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      821 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/image/_sample_average_image_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2111 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/masking/tabular_masker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.554608 attribench-0.1.1/attribench/plot/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      429 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2415 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_cles_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2209 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_cluster_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2715 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_convergence_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5146 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_correlations.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1384 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_krippendorff_alpha_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4183 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_lib.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2089 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_mad_ratio_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      886 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2716 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_wilcoxon_barplot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2722 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/plot/_wilcoxon_summary_plot.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.554608 attribench-0.1.1/attribench/result/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      537 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      430 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_batch_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5982 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_deletion_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      588 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_grouped_batch_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      865 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_grouped_metric_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1934 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_impact_coverage_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2993 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_infidelity_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1369 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_insertion_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1903 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_max_sensitivity_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     6017 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_metric_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3712 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_minimal_subset_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1948 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_parameter_randomization_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3590 2023-07-26 09:26:20.000000 attribench-0.1.1/attribench/result/_sensitivity_n_result.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.582608 attribench-0.1.1/attribench.egg-info/
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2926 2023-07-26 13:18:49.000000 attribench-0.1.1/attribench.egg-info/PKG-INFO
+-rw-rw-r--   0 arne      (1000) arne      (1000)    17755 2023-07-26 13:18:49.000000 attribench-0.1.1/attribench.egg-info/SOURCES.txt
+-rw-rw-r--   0 arne      (1000) arne      (1000)        1 2023-07-26 13:18:49.000000 attribench-0.1.1/attribench.egg-info/dependency_links.txt
+-rw-rw-r--   0 arne      (1000) arne      (1000)      248 2023-07-26 13:18:49.000000 attribench-0.1.1/attribench.egg-info/requires.txt
+-rw-rw-r--   0 arne      (1000) arne      (1000)       11 2023-07-26 13:18:49.000000 attribench-0.1.1/attribench.egg-info/top_level.txt
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.530608 attribench-0.1.1/build/
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.534608 attribench-0.1.1/build/lib/
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.558608 attribench-0.1.1/build/lib/attribench/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      154 2023-07-18 08:49:55.000000 attribench-0.1.1/build/lib/attribench/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      294 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/_activation_fns.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1240 2023-07-18 08:49:02.000000 attribench-0.1.1/build/lib/attribench/_attribution_method.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2808 2023-07-19 12:11:02.000000 attribench-0.1.1/build/lib/attribench/_method_factory.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1274 2023-07-18 08:52:22.000000 attribench-0.1.1/build/lib/attribench/_model_factory.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1528 2023-07-19 14:49:06.000000 attribench-0.1.1/build/lib/attribench/_segmentation.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2866 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/_stat.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.558608 attribench-0.1.1/build/lib/attribench/data/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      323 2023-06-14 14:07:03.000000 attribench-0.1.1/build/lib/attribench/data/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      777 2023-07-19 15:13:56.000000 attribench-0.1.1/build/lib/attribench/data/_index_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      189 2023-07-17 08:32:44.000000 attribench-0.1.1/build/lib/attribench/data/_typing.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.558608 attribench-0.1.1/build/lib/attribench/data/attributions_dataset/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 14:05:47.000000 attribench-0.1.1/build/lib/attribench/data/attributions_dataset/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)    11835 2023-07-19 15:32:55.000000 attribench-0.1.1/build/lib/attribench/data/attributions_dataset/_attributions_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1216 2023-07-19 13:13:40.000000 attribench-0.1.1/build/lib/attribench/data/attributions_dataset/_attributions_dataset_writer.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.558608 attribench-0.1.1/build/lib/attribench/data/hdf5_dataset/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 14:05:51.000000 attribench-0.1.1/build/lib/attribench/data/hdf5_dataset/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1428 2023-07-18 08:56:37.000000 attribench-0.1.1/build/lib/attribench/data/hdf5_dataset/_hdf5_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2323 2023-07-19 13:12:24.000000 attribench-0.1.1/build/lib/attribench/data/hdf5_dataset/_hdf5_dataset_writer.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.558608 attribench-0.1.1/build/lib/attribench/data/nd_array_tree/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 14:05:56.000000 attribench-0.1.1/build/lib/attribench/data/nd_array_tree/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     6081 2023-07-15 15:14:55.000000 attribench-0.1.1/build/lib/attribench/data/nd_array_tree/_nd_array_tree.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)    13407 2023-07-15 15:29:50.000000 attribench-0.1.1/build/lib/attribench/data/nd_array_tree/_random_access_nd_array_tree.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.562608 attribench-0.1.1/build/lib/attribench/distributed/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      198 2023-06-15 05:04:31.000000 attribench-0.1.1/build/lib/attribench/distributed/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5859 2023-07-19 13:14:15.000000 attribench-0.1.1/build/lib/attribench/distributed/_compute_attributions.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2851 2023-07-21 06:47:03.000000 attribench-0.1.1/build/lib/attribench/distributed/_distributed_computation.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      907 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/distributed/_distributed_sampler.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      318 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/distributed/_message.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5584 2023-07-19 13:08:34.000000 attribench-0.1.1/build/lib/attribench/distributed/_select_samples.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5287 2023-07-18 08:56:52.000000 attribench-0.1.1/build/lib/attribench/distributed/_train_adversarial_patches.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2033 2023-07-17 06:25:18.000000 attribench-0.1.1/build/lib/attribench/distributed/_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.566608 attribench-0.1.1/build/lib/attribench/distributed/metrics/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      518 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3098 2023-07-21 13:33:42.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/_metric.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3628 2023-07-19 15:18:56.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/_metric_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.566608 attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 09:44:50.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4718 2023-07-21 06:15:58.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/_deletion.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1410 2023-07-17 13:40:15.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/_deletion_worker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4706 2023-06-15 12:07:07.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/_insertion.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     7166 2023-07-16 07:54:04.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/_irof.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.566608 attribench-0.1.1/build/lib/attribench/distributed/metrics/impact_coverage/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 09:49:05.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/impact_coverage/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3879 2023-07-21 06:23:14.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/impact_coverage/_impact_coverage.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1966 2023-07-17 08:55:17.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/impact_coverage/_impact_coverage_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.566608 attribench-0.1.1/build/lib/attribench/distributed/metrics/infidelity/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-16 07:17:59.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/infidelity/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4663 2023-07-21 06:18:44.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/infidelity/_infidelity.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1526 2023-07-19 15:18:41.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/infidelity/_infidelity_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.566608 attribench-0.1.1/build/lib/attribench/distributed/metrics/max_sensitivity/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 12:27:30.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/max_sensitivity/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3931 2023-07-21 06:22:42.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/max_sensitivity/_max_sensitivity.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1524 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/max_sensitivity/_max_sensitivity_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.570608 attribench-0.1.1/build/lib/attribench/distributed/metrics/minimal_subset/
+-rw-rw-r--   0 arne      (1000) arne      (1000)        0 2023-06-14 12:30:21.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/minimal_subset/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3958 2023-07-21 06:21:52.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/minimal_subset/_minimal_subset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1179 2023-07-16 08:03:42.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/minimal_subset/_minimal_subset_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.570608 attribench-0.1.1/build/lib/attribench/distributed/metrics/sensitivity_n/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       40 2023-07-09 09:02:45.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/sensitivity_n/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5437 2023-07-21 06:20:48.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/sensitivity_n/_sensitivity_n.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2035 2023-07-19 15:32:37.000000 attribench-0.1.1/build/lib/attribench/distributed/metrics/sensitivity_n/_sensitivity_n_worker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.570608 attribench-0.1.1/build/lib/attribench/functional/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      165 2023-06-15 07:07:46.000000 attribench-0.1.1/build/lib/attribench/functional/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3036 2023-07-19 13:06:31.000000 attribench-0.1.1/build/lib/attribench/functional/_compute_attributions.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3270 2023-07-19 11:45:05.000000 attribench-0.1.1/build/lib/attribench/functional/_select_samples.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     7102 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/functional/_train_adversarial_patches.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.570608 attribench-0.1.1/build/lib/attribench/functional/metrics/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      361 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     8740 2023-07-21 06:37:24.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/_impact_coverage.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4216 2023-07-21 06:28:11.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/_insertion.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4617 2023-07-21 06:29:11.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/_irof.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4929 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/_max_sensitivity.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5262 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/_parameter_randomization.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.570608 attribench-0.1.1/build/lib/attribench/functional/metrics/deletion/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       31 2023-06-15 07:51:41.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/deletion/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2751 2023-07-17 13:43:40.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/deletion/_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4504 2023-07-21 13:21:48.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/deletion/_deletion.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      877 2023-06-15 08:15:06.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/deletion/_get_predictions.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.570608 attribench-0.1.1/build/lib/attribench/functional/metrics/infidelity/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      253 2023-07-19 14:12:51.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/infidelity/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     8782 2023-07-21 06:30:12.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/infidelity/_infidelity.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3964 2023-06-16 07:19:46.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/infidelity/_perturbation_generator.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.570608 attribench-0.1.1/build/lib/attribench/functional/metrics/minimal_subset/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       43 2023-06-16 09:37:14.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/minimal_subset/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1663 2023-07-21 06:34:50.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/minimal_subset/_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5525 2023-07-21 06:35:55.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/minimal_subset/_minimal_subset.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.570608 attribench-0.1.1/build/lib/attribench/functional/metrics/sensitivity_n/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       41 2023-07-07 12:54:55.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/sensitivity_n/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2248 2023-07-17 14:18:11.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/sensitivity_n/_dataset.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)    10175 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/functional/metrics/sensitivity_n/_sensitivity_n.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.574608 attribench-0.1.1/build/lib/attribench/masking/
+-rw-rw-r--   0 arne      (1000) arne      (1000)       69 2023-07-17 13:46:49.000000 attribench-0.1.1/build/lib/attribench/masking/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4211 2023-07-18 08:57:40.000000 attribench-0.1.1/build/lib/attribench/masking/_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1110 2023-07-17 12:17:39.000000 attribench-0.1.1/build/lib/attribench/masking/blurring_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      401 2023-07-17 12:17:39.000000 attribench-0.1.1/build/lib/attribench/masking/constant_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     8617 2023-06-15 11:37:49.000000 attribench-0.1.1/build/lib/attribench/masking/image_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1476 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/masking/masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      425 2023-07-17 12:17:39.000000 attribench-0.1.1/build/lib/attribench/masking/random_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      477 2023-07-17 12:17:39.000000 attribench-0.1.1/build/lib/attribench/masking/sample_average_masker.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2111 2023-07-17 13:39:10.000000 attribench-0.1.1/build/lib/attribench/masking/tabular_masker.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.578608 attribench-0.1.1/build/lib/attribench/plot/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      429 2023-07-21 07:44:01.000000 attribench-0.1.1/build/lib/attribench/plot/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2415 2023-07-18 07:40:27.000000 attribench-0.1.1/build/lib/attribench/plot/_cles_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2209 2023-07-18 07:42:07.000000 attribench-0.1.1/build/lib/attribench/plot/_cluster_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2715 2023-07-18 08:58:09.000000 attribench-0.1.1/build/lib/attribench/plot/_convergence_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5146 2023-07-18 07:25:08.000000 attribench-0.1.1/build/lib/attribench/plot/_correlations.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1384 2023-07-18 07:27:47.000000 attribench-0.1.1/build/lib/attribench/plot/_krippendorff_alpha_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4183 2023-07-17 15:26:00.000000 attribench-0.1.1/build/lib/attribench/plot/_lib.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2089 2023-07-18 07:36:12.000000 attribench-0.1.1/build/lib/attribench/plot/_mad_ratio_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      886 2023-07-18 08:58:13.000000 attribench-0.1.1/build/lib/attribench/plot/_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2716 2023-07-18 07:37:09.000000 attribench-0.1.1/build/lib/attribench/plot/_wilcoxon_barplot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2722 2023-07-17 15:35:42.000000 attribench-0.1.1/build/lib/attribench/plot/_wilcoxon_summary_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1157 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/plot/cles_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1631 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/plot/cluster_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1445 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/plot/convergence_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2416 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/plot/correlations.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      866 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/plot/krippendorff_alpha.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     4844 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/plot/lib.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1589 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/attribench/plot/mad_ratio_plot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1185 2023-07-17 14:25:06.000000 attribench-0.1.1/build/lib/attribench/plot/wilcoxon_barplot.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1565 2023-07-17 14:25:06.000000 attribench-0.1.1/build/lib/attribench/plot/wilcoxon_summary_plot.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.578608 attribench-0.1.1/build/lib/attribench/result/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      537 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/result/__init__.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      430 2023-07-13 14:54:39.000000 attribench-0.1.1/build/lib/attribench/result/_batch_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     5982 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/result/_deletion_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      588 2023-07-13 14:52:59.000000 attribench-0.1.1/build/lib/attribench/result/_grouped_batch_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)      865 2023-07-13 14:51:58.000000 attribench-0.1.1/build/lib/attribench/result/_grouped_metric_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1934 2023-07-18 08:58:20.000000 attribench-0.1.1/build/lib/attribench/result/_impact_coverage_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2993 2023-07-18 08:58:26.000000 attribench-0.1.1/build/lib/attribench/result/_infidelity_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1369 2023-07-14 06:15:54.000000 attribench-0.1.1/build/lib/attribench/result/_insertion_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1903 2023-07-18 08:58:30.000000 attribench-0.1.1/build/lib/attribench/result/_max_sensitivity_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     6017 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/result/_metric_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3712 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/result/_minimal_subset_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1948 2023-07-26 07:10:26.000000 attribench-0.1.1/build/lib/attribench/result/_parameter_randomization_result.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     3590 2023-07-21 13:29:34.000000 attribench-0.1.1/build/lib/attribench/result/_sensitivity_n_result.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.534608 attribench-0.1.1/build/lib/docs/
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.578608 attribench-0.1.1/build/lib/docs/source/
+-rw-rw-r--   0 arne      (1000) arne      (1000)     2605 2023-07-18 08:55:42.000000 attribench-0.1.1/build/lib/docs/source/conf.py
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.578608 attribench-0.1.1/build/lib/tests/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      117 2023-06-12 12:11:57.000000 attribench-0.1.1/build/lib/tests/test.py
+-rw-rw-r--   0 arne      (1000) arne      (1000)     1633 2023-07-26 12:33:24.000000 attribench-0.1.1/pyproject.toml
+-rw-rw-r--   0 arne      (1000) arne      (1000)       38 2023-07-26 13:18:49.586608 attribench-0.1.1/setup.cfg
+drwxrwxr-x   0 arne      (1000) arne      (1000)        0 2023-07-26 13:18:49.578608 attribench-0.1.1/tests/
+-rw-rw-r--   0 arne      (1000) arne      (1000)      117 2023-06-12 12:11:57.000000 attribench-0.1.1/tests/test.py
```

### Comparing `attribench-0.1.0/LICENSE` & `attribench-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/PKG-INFO` & `attribench-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attribench
-Version: 0.1.0
+Version: 0.1.1
 Summary: A benchmark for feature attribution techniques
 Author-email: Arne Gevaert <arne.gevaert@ugent.be>, Axel-Jan Rousseau <axeljan.rousseau@uhasselt.be>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,12 +30,33 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
-AttrBench: Metrics for Feature Attribution Techniques
+AttriBench: Metrics for Feature Attribution Techniques
 ======================================================
-**AttrBench** is a [Pytorch](https://pytorch.org/)-based implementation of several metrics for the evaluation of feature attribution maps and methods.
+**AttriBench** is a `Pytorch <https://pytorch.org/>`_-based implementation of
+several metrics for the evaluation of feature attribution maps and methods.
+AttriBench provides a functional and an object-oriented API for the computation
+of these metrics, along with a set of utility functions for the necessary
+preparations (e.g. computing attribution maps) as well as for the visualization
+of the results.
+
+The **functional API** is generally easier to use, and can be used to get
+started quickly if the scale of the evaluation is not too large. The
+**object-oriented API** is more flexible and can use multiple GPUs for
+evaluation of large datasets.
+
+For more information, see the `documentation <https://attribench.readthedocs.io/>`_.
+
+Installation
+------------
+AttriBench can be installed from PyPI using pip:
+
+.. code-block:: bash
+    
+    pip install attribench
```

### Comparing `attribench-0.1.0/attribench/_attribution_method.py` & `attribench-0.1.1/attribench/_attribution_method.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/_method_factory.py` & `attribench-0.1.1/attribench/_method_factory.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/_model_factory.py` & `attribench-0.1.1/attribench/_model_factory.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/_segmentation.py` & `attribench-0.1.1/attribench/_segmentation.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/_stat.py` & `attribench-0.1.1/attribench/_stat.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/data/_index_dataset.py` & `attribench-0.1.1/attribench/data/_index_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/data/attributions_dataset/_attributions_dataset.py` & `attribench-0.1.1/attribench/data/attributions_dataset/_attributions_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/data/attributions_dataset/_attributions_dataset_writer.py` & `attribench-0.1.1/attribench/data/attributions_dataset/_attributions_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/data/hdf5_dataset/_hdf5_dataset.py` & `attribench-0.1.1/attribench/data/hdf5_dataset/_hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/data/hdf5_dataset/_hdf5_dataset_writer.py` & `attribench-0.1.1/attribench/data/hdf5_dataset/_hdf5_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/data/nd_array_tree/_nd_array_tree.py` & `attribench-0.1.1/attribench/data/nd_array_tree/_nd_array_tree.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/data/nd_array_tree/_random_access_nd_array_tree.py` & `attribench-0.1.1/attribench/data/nd_array_tree/_random_access_nd_array_tree.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/_compute_attributions.py` & `attribench-0.1.1/attribench/distributed/_compute_attributions.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/_distributed_computation.py` & `attribench-0.1.1/attribench/distributed/_distributed_computation.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/_distributed_sampler.py` & `attribench-0.1.1/attribench/distributed/_distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/_select_samples.py` & `attribench-0.1.1/attribench/distributed/_select_samples.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/_train_adversarial_patches.py` & `attribench-0.1.1/attribench/distributed/_train_adversarial_patches.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/_worker.py` & `attribench-0.1.1/attribench/distributed/_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/__init__.py` & `attribench-0.1.1/attribench/distributed/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/_metric.py` & `attribench-0.1.1/attribench/distributed/metrics/_metric.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/_metric_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/_metric_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/deletion/_deletion.py` & `attribench-0.1.1/attribench/distributed/metrics/deletion/_deletion.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/deletion/_deletion_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/deletion/_deletion_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/impact_coverage/_impact_coverage.py` & `attribench-0.1.1/attribench/distributed/metrics/impact_coverage/_impact_coverage.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/impact_coverage/_impact_coverage_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/impact_coverage/_impact_coverage_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/infidelity/_infidelity.py` & `attribench-0.1.1/attribench/distributed/metrics/infidelity/_infidelity.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/infidelity/_infidelity_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/infidelity/_infidelity_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/insertion/_insertion.py` & `attribench-0.1.1/attribench/distributed/metrics/insertion/_insertion.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/irof/_irof.py` & `attribench-0.1.1/attribench/distributed/metrics/irof/_irof.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/irof/_irof_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/irof/_irof_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/max_sensitivity/_max_sensitivity.py` & `attribench-0.1.1/attribench/distributed/metrics/max_sensitivity/_max_sensitivity.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/max_sensitivity/_max_sensitivity_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/max_sensitivity/_max_sensitivity_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/minimal_subset/_minimal_subset.py` & `attribench-0.1.1/attribench/distributed/metrics/minimal_subset/_minimal_subset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/minimal_subset/_minimal_subset_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/minimal_subset/_minimal_subset_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/parameter_randomization/_parameter_randomization.py` & `attribench-0.1.1/attribench/distributed/metrics/parameter_randomization/_parameter_randomization.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/parameter_randomization/_parameter_randomization_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/parameter_randomization/_parameter_randomization_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/sensitivity_n/_sensitivity_n.py` & `attribench-0.1.1/attribench/distributed/metrics/sensitivity_n/_sensitivity_n.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/distributed/metrics/sensitivity_n/_sensitivity_n_worker.py` & `attribench-0.1.1/attribench/distributed/metrics/sensitivity_n/_sensitivity_n_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/_compute_attributions.py` & `attribench-0.1.1/attribench/functional/_compute_attributions.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/_select_samples.py` & `attribench-0.1.1/attribench/functional/_select_samples.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/_train_adversarial_patches.py` & `attribench-0.1.1/attribench/functional/_train_adversarial_patches.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/_impact_coverage.py` & `attribench-0.1.1/attribench/functional/metrics/_impact_coverage.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/_insertion.py` & `attribench-0.1.1/attribench/functional/metrics/_insertion.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/_irof.py` & `attribench-0.1.1/attribench/functional/metrics/_irof.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/_max_sensitivity.py` & `attribench-0.1.1/attribench/functional/metrics/_max_sensitivity.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/_parameter_randomization.py` & `attribench-0.1.1/attribench/functional/metrics/_parameter_randomization.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/deletion/_dataset.py` & `attribench-0.1.1/attribench/functional/metrics/deletion/_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/deletion/_deletion.py` & `attribench-0.1.1/attribench/functional/metrics/deletion/_deletion.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/deletion/_get_predictions.py` & `attribench-0.1.1/attribench/functional/metrics/deletion/_get_predictions.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/infidelity/_infidelity.py` & `attribench-0.1.1/attribench/functional/metrics/infidelity/_infidelity.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/infidelity/_perturbation_generator.py` & `attribench-0.1.1/attribench/functional/metrics/infidelity/_perturbation_generator.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/minimal_subset/_dataset.py` & `attribench-0.1.1/attribench/functional/metrics/minimal_subset/_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/minimal_subset/_minimal_subset.py` & `attribench-0.1.1/attribench/functional/metrics/minimal_subset/_minimal_subset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/sensitivity_n/_dataset.py` & `attribench-0.1.1/attribench/functional/metrics/sensitivity_n/_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/functional/metrics/sensitivity_n/_sensitivity_n.py` & `attribench-0.1.1/attribench/functional/metrics/sensitivity_n/_sensitivity_n.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/masking/_masker.py` & `attribench-0.1.1/attribench/masking/_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/masking/image/_blurring_image_masker.py` & `attribench-0.1.1/attribench/masking/image/_blurring_image_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/masking/image/_constant_image_masker.py` & `attribench-0.1.1/attribench/masking/image/_constant_image_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/masking/image/_image_masker.py` & `attribench-0.1.1/attribench/masking/image/_image_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/masking/image/_random_image_masker.py` & `attribench-0.1.1/attribench/masking/image/_random_image_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/masking/image/_sample_average_image_masker.py` & `attribench-0.1.1/attribench/masking/image/_sample_average_image_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/masking/tabular_masker.py` & `attribench-0.1.1/attribench/masking/tabular_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_cles_plot.py` & `attribench-0.1.1/attribench/plot/_cles_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_cluster_plot.py` & `attribench-0.1.1/attribench/plot/_cluster_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_convergence_plot.py` & `attribench-0.1.1/attribench/plot/_convergence_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_correlations.py` & `attribench-0.1.1/attribench/plot/_correlations.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_krippendorff_alpha_plot.py` & `attribench-0.1.1/attribench/plot/_krippendorff_alpha_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_lib.py` & `attribench-0.1.1/attribench/plot/_lib.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_mad_ratio_plot.py` & `attribench-0.1.1/attribench/plot/_mad_ratio_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_plot.py` & `attribench-0.1.1/attribench/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_wilcoxon_barplot.py` & `attribench-0.1.1/attribench/plot/_wilcoxon_barplot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/plot/_wilcoxon_summary_plot.py` & `attribench-0.1.1/attribench/plot/_wilcoxon_summary_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/__init__.py` & `attribench-0.1.1/attribench/result/__init__.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_deletion_result.py` & `attribench-0.1.1/attribench/result/_deletion_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_grouped_batch_result.py` & `attribench-0.1.1/attribench/result/_grouped_batch_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_grouped_metric_result.py` & `attribench-0.1.1/attribench/result/_grouped_metric_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_impact_coverage_result.py` & `attribench-0.1.1/attribench/result/_impact_coverage_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_infidelity_result.py` & `attribench-0.1.1/attribench/result/_infidelity_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_insertion_result.py` & `attribench-0.1.1/attribench/result/_insertion_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_max_sensitivity_result.py` & `attribench-0.1.1/attribench/result/_max_sensitivity_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_metric_result.py` & `attribench-0.1.1/attribench/result/_metric_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_minimal_subset_result.py` & `attribench-0.1.1/attribench/result/_minimal_subset_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_parameter_randomization_result.py` & `attribench-0.1.1/attribench/result/_parameter_randomization_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench/result/_sensitivity_n_result.py` & `attribench-0.1.1/attribench/result/_sensitivity_n_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/attribench.egg-info/PKG-INFO` & `attribench-0.1.1/attribench.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: attribench
-Version: 0.1.0
+Version: 0.1.1
 Summary: A benchmark for feature attribution techniques
 Author-email: Arne Gevaert <arne.gevaert@ugent.be>, Axel-Jan Rousseau <axeljan.rousseau@uhasselt.be>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,12 +30,33 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
+Provides-Extra: docs
 License-File: LICENSE
 
-AttrBench: Metrics for Feature Attribution Techniques
+AttriBench: Metrics for Feature Attribution Techniques
 ======================================================
-**AttrBench** is a [Pytorch](https://pytorch.org/)-based implementation of several metrics for the evaluation of feature attribution maps and methods.
+**AttriBench** is a `Pytorch <https://pytorch.org/>`_-based implementation of
+several metrics for the evaluation of feature attribution maps and methods.
+AttriBench provides a functional and an object-oriented API for the computation
+of these metrics, along with a set of utility functions for the necessary
+preparations (e.g. computing attribution maps) as well as for the visualization
+of the results.
+
+The **functional API** is generally easier to use, and can be used to get
+started quickly if the scale of the evaluation is not too large. The
+**object-oriented API** is more flexible and can use multiple GPUs for
+evaluation of large datasets.
+
+For more information, see the `documentation <https://attribench.readthedocs.io/>`_.
+
+Installation
+------------
+AttriBench can be installed from PyPI using pip:
+
+.. code-block:: bash
+    
+    pip install attribench
```

### Comparing `attribench-0.1.0/attribench.egg-info/SOURCES.txt` & `attribench-0.1.1/attribench.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,14 @@
 ./build/lib/attribench/result/_max_sensitivity_result.py
 ./build/lib/attribench/result/_metric_result.py
 ./build/lib/attribench/result/_minimal_subset_result.py
 ./build/lib/attribench/result/_parameter_randomization_result.py
 ./build/lib/attribench/result/_sensitivity_n_result.py
 ./build/lib/docs/source/conf.py
 ./build/lib/tests/test.py
-./docs/source/conf.py
 ./tests/test.py
 attribench/__init__.py
 attribench/_activation_fns.py
 attribench/_attribution_method.py
 attribench/_method_factory.py
 attribench/_model_factory.py
 attribench/_segmentation.py
```

### Comparing `attribench-0.1.0/build/lib/attribench/_attribution_method.py` & `attribench-0.1.1/build/lib/attribench/_attribution_method.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/_method_factory.py` & `attribench-0.1.1/build/lib/attribench/_method_factory.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/_model_factory.py` & `attribench-0.1.1/build/lib/attribench/_model_factory.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/_segmentation.py` & `attribench-0.1.1/build/lib/attribench/_segmentation.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/_stat.py` & `attribench-0.1.1/build/lib/attribench/_stat.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/data/_index_dataset.py` & `attribench-0.1.1/build/lib/attribench/data/_index_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/data/attributions_dataset/_attributions_dataset.py` & `attribench-0.1.1/build/lib/attribench/data/attributions_dataset/_attributions_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/data/attributions_dataset/_attributions_dataset_writer.py` & `attribench-0.1.1/build/lib/attribench/data/attributions_dataset/_attributions_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/data/hdf5_dataset/_hdf5_dataset.py` & `attribench-0.1.1/build/lib/attribench/data/hdf5_dataset/_hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/data/hdf5_dataset/_hdf5_dataset_writer.py` & `attribench-0.1.1/build/lib/attribench/data/hdf5_dataset/_hdf5_dataset_writer.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/data/nd_array_tree/_nd_array_tree.py` & `attribench-0.1.1/build/lib/attribench/data/nd_array_tree/_nd_array_tree.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/data/nd_array_tree/_random_access_nd_array_tree.py` & `attribench-0.1.1/build/lib/attribench/data/nd_array_tree/_random_access_nd_array_tree.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/_compute_attributions.py` & `attribench-0.1.1/build/lib/attribench/distributed/_compute_attributions.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/_distributed_computation.py` & `attribench-0.1.1/build/lib/attribench/distributed/_distributed_computation.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/_distributed_sampler.py` & `attribench-0.1.1/build/lib/attribench/distributed/_distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/_select_samples.py` & `attribench-0.1.1/build/lib/attribench/distributed/_select_samples.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/_train_adversarial_patches.py` & `attribench-0.1.1/build/lib/attribench/distributed/_train_adversarial_patches.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/_worker.py` & `attribench-0.1.1/build/lib/attribench/distributed/_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/__init__.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/_metric.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/_metric.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/_metric_worker.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/_metric_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/_deletion.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/_deletion.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/_deletion_worker.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/_deletion_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/_insertion.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/_insertion.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/deletion/_irof.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/deletion/_irof.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/impact_coverage/_impact_coverage.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/impact_coverage/_impact_coverage.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/impact_coverage/_impact_coverage_worker.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/impact_coverage/_impact_coverage_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/infidelity/_infidelity.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/infidelity/_infidelity.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/infidelity/_infidelity_worker.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/infidelity/_infidelity_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/max_sensitivity/_max_sensitivity.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/max_sensitivity/_max_sensitivity.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/max_sensitivity/_max_sensitivity_worker.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/max_sensitivity/_max_sensitivity_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/minimal_subset/_minimal_subset.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/minimal_subset/_minimal_subset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/minimal_subset/_minimal_subset_worker.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/minimal_subset/_minimal_subset_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/sensitivity_n/_sensitivity_n.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/sensitivity_n/_sensitivity_n.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/distributed/metrics/sensitivity_n/_sensitivity_n_worker.py` & `attribench-0.1.1/build/lib/attribench/distributed/metrics/sensitivity_n/_sensitivity_n_worker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/_compute_attributions.py` & `attribench-0.1.1/build/lib/attribench/functional/_compute_attributions.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/_select_samples.py` & `attribench-0.1.1/build/lib/attribench/functional/_select_samples.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/_train_adversarial_patches.py` & `attribench-0.1.1/build/lib/attribench/functional/_train_adversarial_patches.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/_impact_coverage.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/_impact_coverage.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/_insertion.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/_insertion.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/_irof.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/_irof.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/_max_sensitivity.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/_max_sensitivity.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/_parameter_randomization.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/_parameter_randomization.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/deletion/_dataset.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/deletion/_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/deletion/_deletion.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/deletion/_deletion.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/deletion/_get_predictions.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/deletion/_get_predictions.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/infidelity/_infidelity.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/infidelity/_infidelity.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/infidelity/_perturbation_generator.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/infidelity/_perturbation_generator.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/minimal_subset/_dataset.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/minimal_subset/_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/minimal_subset/_minimal_subset.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/minimal_subset/_minimal_subset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/sensitivity_n/_dataset.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/sensitivity_n/_dataset.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/functional/metrics/sensitivity_n/_sensitivity_n.py` & `attribench-0.1.1/build/lib/attribench/functional/metrics/sensitivity_n/_sensitivity_n.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/masking/_masker.py` & `attribench-0.1.1/build/lib/attribench/masking/_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/masking/blurring_masker.py` & `attribench-0.1.1/build/lib/attribench/masking/blurring_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/masking/image_masker.py` & `attribench-0.1.1/build/lib/attribench/masking/image_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/masking/masker.py` & `attribench-0.1.1/build/lib/attribench/masking/masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/masking/tabular_masker.py` & `attribench-0.1.1/build/lib/attribench/masking/tabular_masker.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_cles_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/_cles_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_cluster_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/_cluster_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_convergence_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/_convergence_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_correlations.py` & `attribench-0.1.1/build/lib/attribench/plot/_correlations.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_krippendorff_alpha_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/_krippendorff_alpha_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_lib.py` & `attribench-0.1.1/build/lib/attribench/plot/_lib.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_mad_ratio_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/_mad_ratio_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_wilcoxon_barplot.py` & `attribench-0.1.1/build/lib/attribench/plot/_wilcoxon_barplot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/_wilcoxon_summary_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/_wilcoxon_summary_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/cles_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/cles_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/cluster_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/cluster_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/convergence_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/convergence_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/correlations.py` & `attribench-0.1.1/build/lib/attribench/plot/correlations.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/krippendorff_alpha.py` & `attribench-0.1.1/build/lib/attribench/plot/krippendorff_alpha.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/lib.py` & `attribench-0.1.1/build/lib/attribench/plot/lib.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/mad_ratio_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/mad_ratio_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/wilcoxon_barplot.py` & `attribench-0.1.1/build/lib/attribench/plot/wilcoxon_barplot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/plot/wilcoxon_summary_plot.py` & `attribench-0.1.1/build/lib/attribench/plot/wilcoxon_summary_plot.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/__init__.py` & `attribench-0.1.1/build/lib/attribench/result/__init__.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_deletion_result.py` & `attribench-0.1.1/build/lib/attribench/result/_deletion_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_grouped_batch_result.py` & `attribench-0.1.1/build/lib/attribench/result/_grouped_batch_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_grouped_metric_result.py` & `attribench-0.1.1/build/lib/attribench/result/_grouped_metric_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_impact_coverage_result.py` & `attribench-0.1.1/build/lib/attribench/result/_impact_coverage_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_infidelity_result.py` & `attribench-0.1.1/build/lib/attribench/result/_infidelity_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_insertion_result.py` & `attribench-0.1.1/build/lib/attribench/result/_insertion_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_max_sensitivity_result.py` & `attribench-0.1.1/build/lib/attribench/result/_max_sensitivity_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_metric_result.py` & `attribench-0.1.1/build/lib/attribench/result/_metric_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_minimal_subset_result.py` & `attribench-0.1.1/build/lib/attribench/result/_minimal_subset_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_parameter_randomization_result.py` & `attribench-0.1.1/build/lib/attribench/result/_parameter_randomization_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/attribench/result/_sensitivity_n_result.py` & `attribench-0.1.1/build/lib/attribench/result/_sensitivity_n_result.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/build/lib/docs/source/conf.py` & `attribench-0.1.1/build/lib/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `attribench-0.1.0/pyproject.toml` & `attribench-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "attribench"
-version = "0.1.0"
+version = "0.1.1"
 description = "A benchmark for feature attribution techniques"
 readme = "README.rst"
 authors = [
     { name = "Arne Gevaert", email = "arne.gevaert@ugent.be" },
     { name = "Axel-Jan Rousseau", email = "axeljan.rousseau@uhasselt.be" }
 ]
 license = { file = "LICENSE" }
@@ -33,30 +33,32 @@
     "tqdm",
     "pyyaml",
 ]
 requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = [
+    "bumpver",
+    "pytest"
+]
+docs = [
     "sphinx==6.2.1",
     "sphinx-rtd-theme",
     "numpydoc",
     "sphinx-autodoc-typehints",
-    "bumpver",
-    "pytest"
 ]
 
 [project.urls]
 Homepage = "https://github.com/arnegevaert/benchmark"
 Documentation = "http://attribench.readthedocs.io/"
 
 [tool.bumpver]
-current_version = "0.1.0"
+current_version = "0.1.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 commit = true
-tag = true
+tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = ['current_version = "{version}"', 'version = "{version}"']
 "attribench/__init__.py" = ["{version}"]
```

